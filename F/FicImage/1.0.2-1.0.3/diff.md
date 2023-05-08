# Comparing `tmp/FicImage-1.0.2.tar.gz` & `tmp/FicImage-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FicImage-1.0.2.tar", last modified: Mon May  8 21:40:14 2023, max compression
+gzip compressed data, was "FicImage-1.0.3.tar", last modified: Mon May  8 22:28:16 2023, max compression
```

## Comparing `FicImage-1.0.2.tar` & `FicImage-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 21:40:14.265639 FicImage-1.0.2/
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 21:40:14.265639 FicImage-1.0.2/FicImage/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        0 2023-05-06 04:09:38.000000 FicImage-1.0.2/FicImage/__init__.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5275 2023-05-05 16:21:24.000000 FicImage-1.0.2/FicImage/image.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     4022 2023-05-08 21:37:00.000000 FicImage-1.0.2/FicImage/main.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     2277 2023-05-08 16:20:33.000000 FicImage-1.0.2/FicImage/utils.py
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 21:40:14.265639 FicImage-1.0.2/FicImage.egg-info/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      309 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/SOURCES.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/dependency_links.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/entry_points.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/requires.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/top_level.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImage-1.0.2/LICENSE
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 21:40:14.265639 FicImage-1.0.2/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5264 2023-05-07 15:48:12.000000 FicImage-1.0.2/README.md
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      921 2023-05-08 21:39:59.000000 FicImage-1.0.2/pyproject.toml
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-08 21:40:14.269639 FicImage-1.0.2/setup.cfg
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1243 2023-05-08 21:38:31.000000 FicImage-1.0.2/setup.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 22:28:16.159972 FicImage-1.0.3/
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 22:28:16.159972 FicImage-1.0.3/FicImage/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        0 2023-05-06 04:09:38.000000 FicImage-1.0.3/FicImage/__init__.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5514 2023-05-08 22:25:50.000000 FicImage-1.0.3/FicImage/image.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     3925 2023-05-08 22:25:50.000000 FicImage-1.0.3/FicImage/main.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     2271 2023-05-08 22:25:50.000000 FicImage-1.0.3/FicImage/utils.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 22:28:16.159972 FicImage-1.0.3/FicImage.egg-info/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 22:28:16.000000 FicImage-1.0.3/FicImage.egg-info/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      309 2023-05-08 22:28:16.000000 FicImage-1.0.3/FicImage.egg-info/SOURCES.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-08 22:28:16.000000 FicImage-1.0.3/FicImage.egg-info/dependency_links.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-08 22:28:16.000000 FicImage-1.0.3/FicImage.egg-info/entry_points.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-08 22:28:16.000000 FicImage-1.0.3/FicImage.egg-info/requires.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-08 22:28:16.000000 FicImage-1.0.3/FicImage.egg-info/top_level.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImage-1.0.3/LICENSE
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 22:28:16.159972 FicImage-1.0.3/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5264 2023-05-07 15:48:12.000000 FicImage-1.0.3/README.md
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      921 2023-05-08 22:27:42.000000 FicImage-1.0.3/pyproject.toml
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-08 22:28:16.159972 FicImage-1.0.3/setup.cfg
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1243 2023-05-08 22:27:42.000000 FicImage-1.0.3/setup.py
```

### Comparing `FicImage-1.0.2/FicImage/image.py` & `FicImage-1.0.3/FicImage/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,44 +7,49 @@
 from typing import Tuple
 
 
 def get_image_from_url(
 		url: str,
 		image_format: str,
 		compress_images: bool,
-		max_image_size: int
+		max_image_size: int,
+		debug: bool
 ) -> Tuple[bytes, str, str]:
 	"""
 	:param url: The url of the image.
 	:param image_format: The format to convert the image to.
 	:param compress_images: Whether to compress the image or not.
 	:param max_image_size: The maximum size of the image in bytes.
+	:param debug: Whether to print debug messages or not.
 	:return: A tuple of the image data, the image format and the image mime type.
 	"""
 	try:
 		if url.startswith("data:image") and 'base64' in url:
-			print("Base64 image detected")
+			if debug:
+				print("Base64 image detected")
 			head, base64data = url.split(',')
 			file_ext = str(head.split(';')[0].split('/')[1])
 			imgdata = b64decode(base64data)
 			
 			if file_ext.lower() in ("gif", "webp", "svg"):
-				print("GIF/WEBP/SVG image detected, skipping compression")
+				if debug:
+					print("GIF/WEBP/SVG image detected, skipping compression")
 				return imgdata, file_ext, f"image/{file_ext}"
 			
 			elif file_ext.lower() not in ["jpg", "jpeg", "png", "gif", "webp", "svg"]:
-				print(f"Image format {file_ext} not supported, converting to {image_format}")
+				if debug:
+					print(f"Image format {file_ext} not supported, converting to {image_format}")
 				return (
-					_convert_to_new_format(imgdata, image_format).read(),
+					_convert_to_new_format(imgdata, image_format, debug).read(),
 					image_format.lower(),
 					f"image/{image_format.lower()}"
 				)
 			
 			if compress_images:
-				compressed_base64_image = compress_image(BytesIO(imgdata), max_image_size, file_ext)
+				compressed_base64_image = compress_image(BytesIO(imgdata), max_image_size, file_ext, debug)
 				imgdata = PIL_Image_to_bytes(compressed_base64_image, file_ext)
 				
 			return imgdata, file_ext, f"image/{file_ext}"
 		
 		with requests.Session() as session:
 			img = session.get(url, stream=True)
 		
@@ -62,43 +67,48 @@
 				if img_format.lower() == "gif":
 					if PIL_image.info['version'] not in [b"GIF89a", "GIF89a"]:
 						PIL_image.info['version'] = b"GIF89a"
 					return PIL_Image_to_bytes(PIL_image, "GIF"), "gif", "image/gif"
 				return PIL_Image_to_bytes(PIL_image, "WEBP"), "webp", "image/webp"
 	
 			if compress_images:
-				PIL_image = compress_image(image, max_image_size, img_format)
+				PIL_image = compress_image(image, max_image_size, img_format, debug)
 	
 			return PIL_Image_to_bytes(PIL_image, image_format), image_format, f"image/{image_format.lower()}"
 
 	except Exception as e:
 		print("Encountered an error downloading image: " + str(e))
 
 
-def compress_image(image: BytesIO, target_size: int, image_format: str) -> PIL.Image.Image:
+def compress_image(image: BytesIO, target_size: int, image_format: str, debug: bool) -> PIL.Image.Image:
 	image_size = get_size_format(len(image.getvalue()))
-	print(f"Image size: {image_size}")
+	if debug:
+		print(f"Image size: {image_size}")
 
 	big_photo = Image.open(image).convert("RGBA")
 
 	target_pixel_count = 2.8114 * target_size
 	if len(image.getvalue()) > target_size:
-		print(f"Image is greater than {get_size_format(target_size)}, compressing")
+		if debug:
+			print(f"Image is greater than {get_size_format(target_size)}, compressing")
 		scale_factor = target_pixel_count / math.prod(big_photo.size)
 		if scale_factor < 1:
 			x, y = tuple(int(scale_factor * dim) for dim in big_photo.size)
-			print(f"Resizing image dimensions from {big_photo.size} to ({x}, {y})")
+			if debug:
+				print(f"Resizing image dimensions from {big_photo.size} to ({x}, {y})")
 			sml_photo = big_photo.resize((x, y), resample=Image.LANCZOS)
 		else:
 			sml_photo = big_photo
 		compressed_image_size = get_size_format(len(PIL_Image_to_bytes(sml_photo, image_format)))
-		print(f"Compressed image size: {compressed_image_size}")
+		if debug:
+			print(f"Compressed image size: {compressed_image_size}")
 		return sml_photo
 	else:
-		print(f"Image is less than {get_size_format(target_size)}, not compressing")
+		if debug:
+			print(f"Image is less than {get_size_format(target_size)}, not compressing")
 		return big_photo
 
 
 def PIL_Image_to_bytes(
 		pil_image: PIL.Image.Image,
 		image_format: str
 ) -> bytes:
@@ -141,17 +151,18 @@
 	for unit in ["", "K", "M", "G", "T", "P", "E", "Z"]:
 		if b < factor:
 			return f"{b:.2f}{unit}{suffix}"
 		b /= factor
 	return f"{b:.2f}Y{suffix}"
 
 
-def _convert_to_new_format(image_bytestream, image_format: str):
+def _convert_to_new_format(image_bytestream, image_format: str, debug: bool):
 	new_image = BytesIO()
 	try:
 		Image.open(image_bytestream).save(new_image, format=image_format.upper())
 		new_image.name = f'cover.{image_format.lower()}'
 		new_image.seek(0)
 		return new_image
 	except Exception as e:
-		print(f"Encountered an error converting image to {image_format}\nError: {e}")
+		if debug:
+			print(f"Encountered an error converting image to {image_format}\nError: {e}")
 		return image_bytestream
```

### Comparing `FicImage-1.0.2/FicImage/main.py` & `FicImage-1.0.3/FicImage/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,106 @@
-import sys
+import argparse
 import ebooklib
 from ebooklib import epub
 from bs4 import BeautifulSoup
-from FicImage.image import get_image_from_url
-from FicImage.utils import config_check, load_config_json, default_ficimage_settings
+from image import get_image_from_url
+from utils import config_check, load_config_json, default_ficimage_settings
 
 
-def main(path_to_epub: str, config_file_path: str = None) -> None:
+def main() -> None:
 	"""
 	This function updates the FicHub epub file with images.
-	:param path_to_epub: The path to the FicHub epub file.
-	:param config_file_path: The path to the ficimage.json file.
 	:return: None
 	"""
-	if path_to_epub is None:
-		path_to_epub = sys.argv[1]
+	parser = argparse.ArgumentParser(description="Update a FicHub epub file with images.")
+	parser.add_argument("path_to_epub", help="The path to the FicHub epub file.")
+	parser.add_argument("-c", "--config_file_path", help="The path to the ficimage.json file.")
+	parser.add_argument("-d", "--debug", help="Enable debug mode.", action="store_true")
+	args = parser.parse_args()
+	
+	path_to_epub = args.path_to_epub
+	config_file_path = args.config_file_path
+	debug = args.debug
+	
 	try:
-		_ficimage_json_path = sys.argv[2]
-	except IndexError:
-		_ficimage_json_path = None
-	if config_file_path is None:
-		config_file_path = _ficimage_json_path
-		try:
-			book = epub.read_epub(path_to_epub)
-			print(f'Opened {path_to_epub}')
-			
-			(config_file_exists, config_file_location) = config_check(config_file_path)
-			if config_file_exists:
-				ficimage_config = load_config_json(config_file_location)
-			else:
-				ficimage_config = default_ficimage_settings()
-			compress_images_config: bool = ficimage_config.get("compress_images", True)
-			default_image_format_config: str = ficimage_config.get("default_image_format", "JPEG")
-			if str(default_image_format_config).lower() not in ("jpg", "jpeg", "png"):
-				default_image_format_config = "JPEG"
-			max_image_size_config: int = ficimage_config.get("max_image_size", 1_000_000)
-			
-			file_name = path_to_epub.split('/')[-1].split('.')[0]
-			
-			for item in book.get_items_of_type(ebooklib.ITEM_DOCUMENT):
+		book = epub.read_epub(path_to_epub)
+		print(f'Opened {path_to_epub}')
+		
+		(config_file_exists, config_file_location) = config_check(config_file_path)
+		if config_file_exists:
+			ficimage_config = load_config_json(config_file_location)
+		else:
+			ficimage_config = default_ficimage_settings()
+		compress_images_config: bool = ficimage_config.get("compress_images", True)
+		default_image_format_config: str = ficimage_config.get("default_image_format", "JPEG")
+		if str(default_image_format_config).lower() not in ("jpg", "jpeg", "png"):
+			default_image_format_config = "JPEG"
+		max_image_size_config: int = ficimage_config.get("max_image_size", 1_000_000)
+		
+		file_name = path_to_epub.split('/')[-1].split('.')[0]
+		
+		for item in book.get_items_of_type(ebooklib.ITEM_DOCUMENT):
+			try:
+				soup = BeautifulSoup(item.content, "lxml-xml")
+				p_tags = soup.find_all('p')
+				images = [i for i in p_tags if '[img:' in i.text]
+				print(f'Found {len(images)} images in {item.file_name}')
+				# Clean up the images link
+				# Right now they look like this: <p>[img: <a
+				# href="https://i.imgur.com/ABCDEF.jpg" rel="noopener noreferrer">data:image/gif;base64,R0lGODlhA</a>]</p>
+				# But we want to get the link in the href attribute:
 				try:
-					soup = BeautifulSoup(item.content, "lxml-xml")
-					p_tags = soup.find_all('p')
-					images = [i for i in p_tags if '[img:' in i.text]
-					print(f'Found {len(images)} images in {item.file_name}')
-					# Clean up the images link
-					# Right now they look like this: <p>[img: <a
-					# href="https://i.imgur.com/ABCDEF.jpg" rel="noopener noreferrer">data:image/gif;base64,R0lGODlhA</a>]</p>
-					# But we want to get the link in the href attribute:
-					try:
-						for image in images:
-							if image is None:
-								print("NoneType, Skipping")
-							else:
-								item_file_name = item.file_name.split('.')[0]
-								image_link = image.a['href']
-								print(f"[{item_file_name}] Image {images.index(image) + 1} "
-								      f"(out of {len(images)}). Source: {image_link}")
+					for image in images:
+						if image is None:
+							print("NoneType, Skipping")
+						else:
+							item_file_name = item.file_name.split('.')[0]
+							image_link = image.a['href']
+							print(f"[{item_file_name}] Image {images.index(image) + 1} "
+							      f"(out of {len(images)}). Source: {image_link}")
+							
+							try:
+								(
+									image_content,
+									image_extension,
+									image_media_type
+								) = get_image_from_url(
+									url=image_link,
+									image_format=default_image_format_config,
+									compress_images=compress_images_config,
+									max_image_size=max_image_size_config,
+									debug=debug
+								)
+								image_path = f"images/" \
+								             f"{item_file_name}_image_{images.index(image)}.{image_extension.lower()}"
+								new_image = f"<img alt='Image {images.index(image)} from {item.file_name}' " \
+								            f"style='text-align: center; margin: 2em auto; display: block;'" \
+								            f" src='{image_path}' />"
 								
-								try:
-									(
-										image_content,
-										image_extension,
-										image_media_type
-									) = get_image_from_url(
-										url=image_link,
-										image_format=default_image_format_config,
-										compress_images=compress_images_config,
-										max_image_size=max_image_size_config
-									)
-									image_path = f"images/" \
-									             f"{item_file_name}_image_{images.index(image)}.{image_extension.lower()}"
-									new_image = f"<img alt='Image {images.index(image)} from {item.file_name}' " \
-									            f"style='text-align: center; margin: 2em auto; display: block;'" \
-									            f" src='{image_path}' />"
-									
-									img = epub.EpubItem(
-										uid=f"{item_file_name}_{images.index(image)}",
-										file_name=image_path,
-										media_type=image_media_type,
-										content=image_content,
-									)
-									book.add_item(img)
-									image.replace_with(BeautifulSoup(new_image, 'lxml-xml'))
-								except Exception as e:
-									print(f"Error with image {images.index(image) + 1}: {e}, skipping ...")
-						item.content = (str(soup).encode('utf-8'))
-					except Exception as e:
-						print(f'Error while parsing images: {e}')
-				except TypeError:
-					print("NoneType error, skipping ...")
-			
-			try:
-				epub.write_epub(f"[FicImage]{file_name}.epub", book)
-				print(f'Wrote [FicImage]{file_name}.epub')
-			except Exception as e:
-				print(f'Error while writing epub: {e}')
-		except FileNotFoundError:
-			print(f'File {path_to_epub} not found.')
-			return
+								img = epub.EpubItem(
+									uid=f"{item_file_name}_{images.index(image)}",
+									file_name=image_path,
+									media_type=image_media_type,
+									content=image_content,
+								)
+								book.add_item(img)
+								image.replace_with(BeautifulSoup(new_image, 'lxml-xml'))
+							except Exception as e:
+								print(f"Error with image {images.index(image) + 1}: {e}, skipping ...")
+					item.content = (str(soup).encode('utf-8'))
+				except Exception as e:
+					print(f'Error while parsing images: {e}')
+			except TypeError:
+				print("NoneType error, skipping ...")
+		
+		try:
+			epub.write_epub(f"[FicImage]{file_name}.epub", book)
+			print(f'Wrote [FicImage]{file_name}.epub')
+		except Exception as e:
+			print(f'Error while writing epub: {e}')
+	except FileNotFoundError:
+		print(f'File {path_to_epub} not found.')
+		return
 
 
 if __name__ == '__main__':
-	try:
-		ficimage_json_path = sys.argv[2]
-	except IndexError:
-		ficimage_json_path = None
-	main(sys.argv[1], ficimage_json_path)
+	main()
```

### Comparing `FicImage-1.0.2/FicImage/utils.py` & `FicImage-1.0.3/FicImage/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 	:param directory_path: A string or None
 	:return: A tuple containing a boolean and a string
 	"""
 	if directory_path is None:
 		current_dir = os.getcwd()
 		print(f"[Config File Check]: No directory was passed, checking current directory '{current_dir}'")
 		
-		file_path = os.path.join(current_dir, "../ficimage.json")
+		file_path = os.path.join(current_dir, "ficimage.json")
 		
 		if os.path.isfile(file_path):
 			print(f"[Config File Check]: ficimage.json found in current directory!")
 			return True, current_dir
 		
 		directory_path = os.path.expanduser("~")
 		print(f"[Config File Check]: ficimage.json not found in current directory, checking '{directory_path}'")
 	
-	file_path = os.path.join(directory_path, "../ficimage.json")
+	file_path = os.path.join(directory_path, "ficimage.json")
 	
 	is_file = os.path.isfile(file_path)
 	print(f"[Config File Check]: "
 	      f"{'ficimage.json found!' if is_file else 'ficimage.json not found, using default config settings'}")
 	
 	return is_file, directory_path
```

### Comparing `FicImage-1.0.2/FicImage.egg-info/PKG-INFO` & `FicImage-1.0.3/FicImage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImage
-Version: 1.0.2
+Version: 1.0.3
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
```

### Comparing `FicImage-1.0.2/LICENSE` & `FicImage-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FicImage-1.0.2/PKG-INFO` & `FicImage-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImage
-Version: 1.0.2
+Version: 1.0.3
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
```

### Comparing `FicImage-1.0.2/README.md` & `FicImage-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `FicImage-1.0.2/pyproject.toml` & `FicImage-1.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "FicImage"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Emmanuel C. Jemeni", email="jemenichinonso11@gmail.com" }
 ]
 description = "FicImage is an application designed to enhance the reading experience of FicHub epubs."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
```

### Comparing `FicImage-1.0.2/setup.py` & `FicImage-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="FicImage",
-	version="1.0.2",
+	version="1.0.3",
 	author="Emmanuel C. Jemeni",
 	author_email="jemenichinonso11@gmail.com",
 	description="FicImage is an application designed to enhance the reading experience of FicHub epubs.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/Jemeni11/FicImage",
 	project_urls={
```

