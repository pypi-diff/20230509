# Comparing `tmp/webuiapi-0.6.2-py3-none-any.whl.zip` & `tmp/webuiapi-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 11707 bytes, number of entries: 7
--rw-r--r--  2.0 unx      484 b- defN 23-Mar-16 11:12 webuiapi/__init__.py
--rw-r--r--  2.0 unx    31305 b- defN 23-Mar-16 11:12 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Mar-16 11:12 webuiapi-0.6.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    12458 b- defN 23-Mar-16 11:12 webuiapi-0.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 11:12 webuiapi-0.6.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-16 11:12 webuiapi-0.6.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-Mar-16 11:12 webuiapi-0.6.2.dist-info/RECORD
-7 files, 45972 bytes uncompressed, 10745 bytes compressed:  76.6%
+Zip file size: 11970 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      484 b- defN 23-May-09 15:10 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    32110 b- defN 23-May-09 15:09 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12778 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      545 b- defN 23-May-09 15:17 webuiapi-0.7.0.dist-info/RECORD
+7 files, 47097 bytes uncompressed, 11008 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.6.2.dist-info/LICENSE
+Filename: webuiapi-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.6.2.dist-info/METADATA
+Filename: webuiapi-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.6.2.dist-info/WHEEL
+Filename: webuiapi-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.6.2.dist-info/top_level.txt
+Filename: webuiapi-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.6.2.dist-info/RECORD
+Filename: webuiapi-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webuiapi/__init__.py

```diff
@@ -1,10 +1,10 @@
 from .webuiapi import WebUIApi, WebUIApiResult, Upscaler, HiResUpscaler, b64_img, raw_b64_img, ModelKeywordResult, ModelKeywordInterface, InstructPix2PixInterface, ControlNetInterface, ControlNetUnit
 
-__version__ = "0.6.2"
+__version__ = "0.7.0"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
```

## webuiapi/webuiapi.py

```diff
@@ -49,58 +49,65 @@
 class ControlNetUnit:
     def __init__(self,
         input_image: Image = None,
         mask: Image = None,
         module: str = "none",
         model: str = "None",
         weight: float = 1.0,
-        resize_mode: str = "Scale to Fit (Inner Fit)",
+        resize_mode: str = "Resize and Fill",
         lowvram: bool = False,
-        processor_res: int = 64,
+        processor_res: int = 512,
         threshold_a: float = 64,
         threshold_b: float = 64,
         guidance: float = 1.0,
         guidance_start: float = 0.0,
         guidance_end: float = 1.0,
-        guessmode: bool = False):
+        control_mode: int = 0,
+        pixel_perfect: bool = False,
+        guessmode: int = None, # deprecated: use control_mode
+        ):
         
         self.input_image = input_image
         self.mask = mask
         self.module = module
         self.model = model
         self.weight = weight
         self.resize_mode = resize_mode
         self.lowvram = lowvram
         self.processor_res = processor_res
         self.threshold_a = threshold_a
         self.threshold_b = threshold_b
         self.guidance = guidance
         self.guidance_start = guidance_start
         self.guidance_end = guidance_end
-        self.guessmode = guessmode
+        if guessmode:
+            print('ControlNetUnit guessmode is deprecated. Please use control_mode instead.')
+            control_mode = guessmode
+        self.control_mode = control_mode
+        self.pixel_perfect = pixel_perfect
 
     def to_dict(self):
         return {
             "input_image": raw_b64_img(self.input_image) if self.input_image else "",
-            "mask": raw_b64_img(self.mask) if self.mask else "",
+            "mask": raw_b64_img(self.mask) if self.mask is not None else None,
             "module": self.module,
             "model": self.model,
             "weight": self.weight,
             "resize_mode": self.resize_mode,
             "lowvram": self.lowvram,
             "processor_res": self.processor_res,
             "threshold_a": self.threshold_a,
             "threshold_b": self.threshold_b,
             "guidance": self.guidance,
             "guidance_start": self.guidance_start,
             "guidance_end": self.guidance_end,
-            "guessmode": self.guessmode,
+            "control_mode": self.control_mode,
+            "pixel_perfect": self.pixel_perfect,
         }
 
-
 def b64_img(image: Image):
     buffered = io.BytesIO()
     image.save(buffered, format="PNG")
     img_base64 = 'data:image/png;base64,' + str(base64.b64encode(buffered.getvalue()), 'utf-8')
     return img_base64
 
 def raw_b64_img(image: Image):
@@ -149,14 +156,16 @@
         if 'info' in r.keys():
             try:
                 info = json.loads(r['info'])
             except:
                 info = r['info']
         elif 'html_info' in r.keys():
             info = r['html_info']
+        elif 'caption' in r.keys():
+            info = r['caption']
 
         parameters = ''
         if 'parameters' in r.keys():
             parameters = r['parameters']
 
         return WebUIApiResult(images, parameters, info)
 
@@ -549,14 +558,26 @@
         response = self.session.get(url=url)
         return response.json()
     def custom_post(self, endpoint, payload={}, baseurl=False):
         url = self.get_endpoint(endpoint, baseurl)
         response = self.session.post(url=url, json=payload)
         return self._to_api_result(response)
 
+    def controlnet_version(self):
+        r = self.custom_get('controlnet/version')
+        return r['version']
+
+    def controlnet_model_list(self):
+        r = self.custom_get('controlnet/model_list')
+        return r['model_list']
+    
+    def controlnet_module_list(self):
+        r = self.custom_get('controlnet/module_list')
+        return r['module_list']
+    
     def util_get_model_names(self):
         return sorted([x['title'] for x in self.get_sd_models()])
     def util_set_model(self, name, find_closest=True):
         if find_closest:
             name = name.lower()
         models = self.util_get_model_names()
         found_model = None
```

## Comparing `webuiapi-0.6.2.dist-info/LICENSE` & `webuiapi-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.6.2.dist-info/METADATA` & `webuiapi-0.7.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.6.2
+Version: 0.7.0
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
 Requires-Python: >=3.7, <4
@@ -329,61 +329,69 @@
 mki.get_keywords()
 ```
 ModelKeywordResult(keywords=['nousr robot'], model='robo-diffusion-v1.ckpt', oldhash='41fef4bd', match_source='model-keyword.txt')
 
 
 ### Extension support - Instruct-Pix2Pix
 ```
-# https://github.com/Klace/stable-diffusion-webui-instruct-pix2pix
-ip2p = webuiapi.InstructPix2PixInterface(api)
-r = ip2p.img2img(prompt='sunset', images=[pil_img], text_cfg=7.5, image_cfg=1.5)
+# Instruct-Pix2Pix extension is now deprecated and is now part of webui.
+# You can use normal img2img with image_cfg_scale when instruct-pix2pix model is loaded.
+r = api.img2img(prompt='sunset', images=[pil_img], cfg_scale=7.5, image_cfg_scale=1.5)
 r.image
 ```
 
 ### Extension support - ControlNet
 ```
 # https://github.com/Mikubill/sd-webui-controlnet
-cn = webuiapi.ControlNetInterface(api)
-cn.model_list()
+
+api.controlnet_model_list()
 ```
 <pre>
-['control_canny-fp16 [e3fe7712]',
- 'control_depth-fp16 [400750f6]',
- 'control_hed-fp16 [13fee50b]',
- 'control_mlsd-fp16 [e3705cfa]',
- 'control_normal-fp16 [63f96f7c]',
- 'control_openpose-fp16 [9ca67cc5]',
- 'control_scribble-fp16 [c508311e]',
- 'control_seg-fp16 [b9c1cc12]']
+['control_v11e_sd15_ip2p [c4bb465c]',
+ 'control_v11e_sd15_shuffle [526bfdae]',
+ 'control_v11f1p_sd15_depth [cfd03158]',
+ 'control_v11p_sd15_canny [d14c016b]',
+ 'control_v11p_sd15_inpaint [ebff9138]',
+ 'control_v11p_sd15_lineart [43d4be0d]',
+ 'control_v11p_sd15_mlsd [aca30ff0]',
+ 'control_v11p_sd15_normalbae [316696f1]',
+ 'control_v11p_sd15_openpose [cab727d4]',
+ 'control_v11p_sd15_scribble [d4ba51ff]',
+ 'control_v11p_sd15_seg [e1f51eb9]',
+ 'control_v11p_sd15_softedge [a8575a2a]',
+ 'control_v11p_sd15s2_lineart_anime [3825e83e]',
+ 'control_v11u_sd15_tile [1f041471]']
  </pre>
 
-**Use of ControlNetInterface txt2img/img2img is deprecated.** Please use the txt2img and img2img api with controlnet_units parameter.
-
+```
+api.controlnet_version()
+api.controlnet_module_list()
+```
 
 ```
 # normal txt2img
 r = api.txt2img(prompt="photo of a beautiful girl with blonde hair", height=512, seed=100)
 img = r.image
 img
 ```
 ![cn1](https://user-images.githubusercontent.com/1288793/222315754-43c6dc8c-2a62-4a31-b51a-f68523118e0d.png)
 
 ```
-# txt2img with ControlNet
+# txt2img with ControlNet (used 1.0 but also supports 2.0)
 unit1 = webuiapi.ControlNetUnit(input_image=img, module='canny', model='control_canny-fp16 [e3fe7712]')
 
 r = api.txt2img(prompt="photo of a beautiful girl", controlnet_units=[unit1])
 r.image
 ```
 
 ![cn2](https://user-images.githubusercontent.com/1288793/222315791-c6c480eb-2987-4044-b673-5f2cb6135f87.png)
 
 
 ```
-# img2img with multiple ControlNets
+# img2img with multiple ControlNets (used 1.0 but also supports 2.0)
 unit1 = webuiapi.ControlNetUnit(input_image=img, module='canny', model='control_canny-fp16 [e3fe7712]')
 unit2 = webuiapi.ControlNetUnit(input_image=img, module='depth', model='control_depth-fp16 [400750f6]', weight=0.5)
 
 r2 = api.img2img(prompt="girl",
             images=[img], 
             width=512,
             height=512,
```

## Comparing `webuiapi-0.6.2.dist-info/RECORD` & `webuiapi-0.7.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-webuiapi/__init__.py,sha256=gGO8GHdJD8Z64Zg7L6PkOAyDCIwP0WR2keE-V5sabCk,484
-webuiapi/webuiapi.py,sha256=_CYVLfIGt0da6oXR63k4si4B7piVcWaYFPxyTyjLd7A,31305
-webuiapi-0.6.2.dist-info/LICENSE,sha256=Zl3ztitjIWviypQXfHYvUR099Y5IUOh15IVxAOw9XV8,1079
-webuiapi-0.6.2.dist-info/METADATA,sha256=RaVNCNYoqmlX5BmoSY5GqhOcsk6vSVHB_fL3oXoFLVc,12458
-webuiapi-0.6.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-webuiapi-0.6.2.dist-info/top_level.txt,sha256=84RprjAaGWFS3oujg2AE1dTHp6o4yGT9isvN6frk5p4,9
-webuiapi-0.6.2.dist-info/RECORD,,
+webuiapi/__init__.py,sha256=4EVXOgYPVLafpooONJeYcND6YS3lD2ocnr6kYzyQeh0,484
+webuiapi/webuiapi.py,sha256=z8S_aA_0axSv4D4WC4Bv1pJa7NGHrs--YkHiiFwZhq4,32110
+webuiapi-0.7.0.dist-info/LICENSE,sha256=Zl3ztitjIWviypQXfHYvUR099Y5IUOh15IVxAOw9XV8,1079
+webuiapi-0.7.0.dist-info/METADATA,sha256=cDfExbwngvQBPcqQU66wu-0oskREp48RQgxCM91qtos,12778
+webuiapi-0.7.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+webuiapi-0.7.0.dist-info/top_level.txt,sha256=84RprjAaGWFS3oujg2AE1dTHp6o4yGT9isvN6frk5p4,9
+webuiapi-0.7.0.dist-info/RECORD,,
```

