# Comparing `tmp/FicImage-1.0.1.tar.gz` & `tmp/FicImage-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FicImage-1.0.1.tar", last modified: Mon May  8 16:26:47 2023, max compression
+gzip compressed data, was "FicImage-1.0.2.tar", last modified: Mon May  8 21:40:14 2023, max compression
```

## Comparing `FicImage-1.0.1.tar` & `FicImage-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 16:26:47.143530 FicImage-1.0.1/
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 16:26:47.143530 FicImage-1.0.1/FicImage/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        0 2023-05-06 04:09:38.000000 FicImage-1.0.1/FicImage/__init__.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5275 2023-05-05 16:21:24.000000 FicImage-1.0.1/FicImage/image.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     3721 2023-05-08 16:20:33.000000 FicImage-1.0.1/FicImage/main.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     2277 2023-05-08 16:20:33.000000 FicImage-1.0.1/FicImage/utils.py
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 16:26:47.143530 FicImage-1.0.1/FicImage.egg-info/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      309 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/SOURCES.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/dependency_links.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/entry_points.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/requires.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-08 16:26:47.000000 FicImage-1.0.1/FicImage.egg-info/top_level.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImage-1.0.1/LICENSE
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 16:26:47.143530 FicImage-1.0.1/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5264 2023-05-07 15:48:12.000000 FicImage-1.0.1/README.md
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      921 2023-05-08 16:26:37.000000 FicImage-1.0.1/pyproject.toml
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-08 16:26:47.143530 FicImage-1.0.1/setup.cfg
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1243 2023-05-08 16:26:37.000000 FicImage-1.0.1/setup.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 21:40:14.265639 FicImage-1.0.2/
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 21:40:14.265639 FicImage-1.0.2/FicImage/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        0 2023-05-06 04:09:38.000000 FicImage-1.0.2/FicImage/__init__.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5275 2023-05-05 16:21:24.000000 FicImage-1.0.2/FicImage/image.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     4022 2023-05-08 21:37:00.000000 FicImage-1.0.2/FicImage/main.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     2277 2023-05-08 16:20:33.000000 FicImage-1.0.2/FicImage/utils.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 21:40:14.265639 FicImage-1.0.2/FicImage.egg-info/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      309 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/SOURCES.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/dependency_links.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/entry_points.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/requires.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-08 21:40:14.000000 FicImage-1.0.2/FicImage.egg-info/top_level.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImage-1.0.2/LICENSE
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     7307 2023-05-08 21:40:14.265639 FicImage-1.0.2/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5264 2023-05-07 15:48:12.000000 FicImage-1.0.2/README.md
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      921 2023-05-08 21:39:59.000000 FicImage-1.0.2/pyproject.toml
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-08 21:40:14.269639 FicImage-1.0.2/setup.cfg
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1243 2023-05-08 21:38:31.000000 FicImage-1.0.2/setup.py
```

### Comparing `FicImage-1.0.1/FicImage/image.py` & `FicImage-1.0.2/FicImage/image.py`

 * *Files identical despite different names*

### Comparing `FicImage-1.0.1/FicImage/main.py` & `FicImage-1.0.2/FicImage/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,92 +9,100 @@
 def main(path_to_epub: str, config_file_path: str = None) -> None:
 	"""
 	This function updates the FicHub epub file with images.
 	:param path_to_epub: The path to the FicHub epub file.
 	:param config_file_path: The path to the ficimage.json file.
 	:return: None
 	"""
+	if path_to_epub is None:
+		path_to_epub = sys.argv[1]
 	try:
-		book = epub.read_epub(path_to_epub)
-		print(f'Opened {path_to_epub}')
-		
-		(config_file_exists, config_file_location) = config_check(config_file_path)
-		if config_file_exists:
-			ficimage_config = load_config_json(config_file_location)
-		else:
-			ficimage_config = default_ficimage_settings()
-		compress_images_config: bool = ficimage_config.get("compress_images", True)
-		default_image_format_config: str = ficimage_config.get("default_image_format", "JPEG")
-		if str(default_image_format_config).lower() not in ("jpg", "jpeg", "png"):
-			default_image_format_config = "JPEG"
-		max_image_size_config: int = ficimage_config.get("max_image_size", 1_000_000)
-		
-		file_name = path_to_epub.split('/')[-1].split('.')[0]
-		
-		for item in book.get_items_of_type(ebooklib.ITEM_DOCUMENT):
-			try:
-				soup = BeautifulSoup(item.content, "lxml-xml")
-				p_tags = soup.find_all('p')
-				images = [i for i in p_tags if '[img:' in i.text]
-				print(f'Found {len(images)} images in {item.file_name}')
-				# Clean up the images link
-				# Right now they look like this: <p>[img: <a
-				# href="https://i.imgur.com/ABCDEF.jpg" rel="noopener noreferrer">data:image/gif;base64,R0lGODlhA</a>]</p>
-				# But we want to get the link in the href attribute:
+		_ficimage_json_path = sys.argv[2]
+	except IndexError:
+		_ficimage_json_path = None
+	if config_file_path is None:
+		config_file_path = _ficimage_json_path
+		try:
+			book = epub.read_epub(path_to_epub)
+			print(f'Opened {path_to_epub}')
+			
+			(config_file_exists, config_file_location) = config_check(config_file_path)
+			if config_file_exists:
+				ficimage_config = load_config_json(config_file_location)
+			else:
+				ficimage_config = default_ficimage_settings()
+			compress_images_config: bool = ficimage_config.get("compress_images", True)
+			default_image_format_config: str = ficimage_config.get("default_image_format", "JPEG")
+			if str(default_image_format_config).lower() not in ("jpg", "jpeg", "png"):
+				default_image_format_config = "JPEG"
+			max_image_size_config: int = ficimage_config.get("max_image_size", 1_000_000)
+			
+			file_name = path_to_epub.split('/')[-1].split('.')[0]
+			
+			for item in book.get_items_of_type(ebooklib.ITEM_DOCUMENT):
 				try:
-					for image in images:
-						if image is None:
-							print("NoneType, Skipping")
-						else:
-							item_file_name = item.file_name.split('.')[0]
-							image_link = image.a['href']
-							print(f"[{item_file_name}] Image {images.index(image) + 1} "
-							      f"(out of {len(images)}). Source: {image_link}")
-	
-							try:
-								(
-									image_content,
-									image_extension,
-									image_media_type
-								) = get_image_from_url(
-									url=image_link,
-									image_format=default_image_format_config,
-									compress_images=compress_images_config,
-									max_image_size=max_image_size_config
-								)
-								image_path = f"images/" \
-								             f"{item_file_name}_image_{images.index(image)}.{image_extension.lower()}"
-								new_image = f"<img alt='Image {images.index(image)} from {item.file_name}' " \
-								            f"style='text-align: center; margin: 2em auto; display: block;'" \
-								            f" src='{image_path}' />"
+					soup = BeautifulSoup(item.content, "lxml-xml")
+					p_tags = soup.find_all('p')
+					images = [i for i in p_tags if '[img:' in i.text]
+					print(f'Found {len(images)} images in {item.file_name}')
+					# Clean up the images link
+					# Right now they look like this: <p>[img: <a
+					# href="https://i.imgur.com/ABCDEF.jpg" rel="noopener noreferrer">data:image/gif;base64,R0lGODlhA</a>]</p>
+					# But we want to get the link in the href attribute:
+					try:
+						for image in images:
+							if image is None:
+								print("NoneType, Skipping")
+							else:
+								item_file_name = item.file_name.split('.')[0]
+								image_link = image.a['href']
+								print(f"[{item_file_name}] Image {images.index(image) + 1} "
+								      f"(out of {len(images)}). Source: {image_link}")
 								
-								img = epub.EpubItem(
-									uid=f"{item_file_name}_{images.index(image)}",
-									file_name=image_path,
-									media_type=image_media_type,
-									content=image_content,
-								)
-								book.add_item(img)
-								image.replace_with(BeautifulSoup(new_image, 'lxml-xml'))
-							except Exception as e:
-								print(f"Error with image {images.index(image) + 1}: {e}, skipping ...")
-					item.content = (str(soup).encode('utf-8'))
-				except Exception as e:
-					print(f'Error while parsing images: {e}')
-			except TypeError:
-				print("NoneType error, skipping ...")
-		
-		try:
-			epub.write_epub(f"[FicImage]{file_name}.epub", book)
-			print(f'Wrote [FicImage]{file_name}.epub')
-		except Exception as e:
-			print(f'Error while writing epub: {e}')
-	except FileNotFoundError:
-		print(f'File {path_to_epub} not found.')
-		return
+								try:
+									(
+										image_content,
+										image_extension,
+										image_media_type
+									) = get_image_from_url(
+										url=image_link,
+										image_format=default_image_format_config,
+										compress_images=compress_images_config,
+										max_image_size=max_image_size_config
+									)
+									image_path = f"images/" \
+									             f"{item_file_name}_image_{images.index(image)}.{image_extension.lower()}"
+									new_image = f"<img alt='Image {images.index(image)} from {item.file_name}' " \
+									            f"style='text-align: center; margin: 2em auto; display: block;'" \
+									            f" src='{image_path}' />"
+									
+									img = epub.EpubItem(
+										uid=f"{item_file_name}_{images.index(image)}",
+										file_name=image_path,
+										media_type=image_media_type,
+										content=image_content,
+									)
+									book.add_item(img)
+									image.replace_with(BeautifulSoup(new_image, 'lxml-xml'))
+								except Exception as e:
+									print(f"Error with image {images.index(image) + 1}: {e}, skipping ...")
+						item.content = (str(soup).encode('utf-8'))
+					except Exception as e:
+						print(f'Error while parsing images: {e}')
+				except TypeError:
+					print("NoneType error, skipping ...")
+			
+			try:
+				epub.write_epub(f"[FicImage]{file_name}.epub", book)
+				print(f'Wrote [FicImage]{file_name}.epub')
+			except Exception as e:
+				print(f'Error while writing epub: {e}')
+		except FileNotFoundError:
+			print(f'File {path_to_epub} not found.')
+			return
 
 
 if __name__ == '__main__':
 	try:
 		ficimage_json_path = sys.argv[2]
 	except IndexError:
 		ficimage_json_path = None
```

### Comparing `FicImage-1.0.1/FicImage/utils.py` & `FicImage-1.0.2/FicImage/utils.py`

 * *Files identical despite different names*

### Comparing `FicImage-1.0.1/FicImage.egg-info/PKG-INFO` & `FicImage-1.0.2/FicImage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImage
-Version: 1.0.1
+Version: 1.0.2
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
```

### Comparing `FicImage-1.0.1/LICENSE` & `FicImage-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FicImage-1.0.1/PKG-INFO` & `FicImage-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImage
-Version: 1.0.1
+Version: 1.0.2
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
```

### Comparing `FicImage-1.0.1/README.md` & `FicImage-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FicImage-1.0.1/pyproject.toml` & `FicImage-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "FicImage"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Emmanuel C. Jemeni", email="jemenichinonso11@gmail.com" }
 ]
 description = "FicImage is an application designed to enhance the reading experience of FicHub epubs."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
```

### Comparing `FicImage-1.0.1/setup.py` & `FicImage-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="FicImage",
-	version="1.0.1",
+	version="1.0.2",
 	author="Emmanuel C. Jemeni",
 	author_email="jemenichinonso11@gmail.com",
 	description="FicImage is an application designed to enhance the reading experience of FicHub epubs.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/Jemeni11/FicImage",
 	project_urls={
```

