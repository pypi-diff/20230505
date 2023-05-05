# Comparing `tmp/PDFVisor-0.1.0.tar.gz` & `tmp/PDFVisor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDFVisor-0.1.0.tar", last modified: Mon Apr 24 15:29:00 2023, max compression
+gzip compressed data, was "PDFVisor-0.1.1.tar", last modified: Fri May  5 15:23:53 2023, max compression
```

## Comparing `PDFVisor-0.1.0.tar` & `PDFVisor-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 15:29:00.381950 PDFVisor-0.1.0/
--rw-rw-rw-   0        0        0      888 2023-03-30 11:59:18.000000 PDFVisor-0.1.0/LICENSE.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 15:29:00.359096 PDFVisor-0.1.0/PDFVisor.egg-info/
--rw-rw-rw-   0        0        0     1478 2023-04-24 15:29:00.000000 PDFVisor-0.1.0/PDFVisor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-04-24 15:29:00.000000 PDFVisor-0.1.0/PDFVisor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 15:29:00.000000 PDFVisor-0.1.0/PDFVisor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-24 15:29:00.000000 PDFVisor-0.1.0/PDFVisor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 15:29:00.000000 PDFVisor-0.1.0/PDFVisor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1478 2023-04-24 15:29:00.380919 PDFVisor-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2023-03-29 11:56:39.000000 PDFVisor-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 15:29:00.381950 PDFVisor-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1793 2023-04-24 15:18:00.000000 PDFVisor-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:29:00.364424 PDFVisor-0.1.0/src/
--rw-rw-rw-   0        0        0     9302 2023-04-24 13:56:08.000000 PDFVisor-0.1.0/src/PDFViewr.py
--rw-rw-rw-   0        0        0        0 2023-04-07 17:56:51.000000 PDFVisor-0.1.0/src/__init__.py
--rw-rw-rw-   0        0        0     4113 2023-04-14 20:56:09.000000 PDFVisor-0.1.0/src/funcsVisorPDF.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:29:00.378858 PDFVisor-0.1.0/src/img/
--rw-rw-rw-   0        0        0     5334 2023-03-26 17:45:11.000000 PDFVisor-0.1.0/src/img/avanceDeshabilitado.png
--rw-rw-rw-   0        0        0     4026 2023-03-26 18:02:13.000000 PDFVisor-0.1.0/src/img/avanceHighlight.png
--rw-rw-rw-   0        0        0     5505 2023-03-26 17:45:11.000000 PDFVisor-0.1.0/src/img/avanceNormal.png
--rw-rw-rw-   0        0        0     5123 2023-03-26 17:45:11.000000 PDFVisor-0.1.0/src/img/avancePressed.png
--rw-rw-rw-   0        0        0     5359 2023-03-26 17:45:11.000000 PDFVisor-0.1.0/src/img/retroDeshabilitado.png
--rw-rw-rw-   0        0        0     4034 2023-03-26 17:45:11.000000 PDFVisor-0.1.0/src/img/retroHighlight.png
--rw-rw-rw-   0        0        0     5540 2023-03-26 17:45:11.000000 PDFVisor-0.1.0/src/img/retroNormal.png
--rw-rw-rw-   0        0        0     5036 2023-03-26 18:06:13.000000 PDFVisor-0.1.0/src/img/retroPressed.png
+drwxrwxrwx   0        0        0        0 2023-05-05 15:23:52.994635 PDFVisor-0.1.1/
+-rw-rw-rw-   0        0        0      888 2023-03-30 11:59:20.000000 PDFVisor-0.1.1/LICENSE.rst
+-rw-rw-rw-   0        0        0       60 2023-05-05 14:14:13.000000 PDFVisor-0.1.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-05 15:23:52.884789 PDFVisor-0.1.1/PDFVisor.egg-info/
+-rw-rw-rw-   0        0        0     1478 2023-05-05 15:23:52.000000 PDFVisor-0.1.1/PDFVisor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-05-05 15:23:52.000000 PDFVisor-0.1.1/PDFVisor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 15:23:52.000000 PDFVisor-0.1.1/PDFVisor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-05 15:23:52.000000 PDFVisor-0.1.1/PDFVisor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 15:23:52.000000 PDFVisor-0.1.1/PDFVisor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1478 2023-05-05 15:23:52.994635 PDFVisor-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-03-29 11:56:40.000000 PDFVisor-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 15:23:52.994635 PDFVisor-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1815 2023-05-01 15:37:31.000000 PDFVisor-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:23:52.916461 PDFVisor-0.1.1/src/
+-rw-rw-rw-   0        0        0     9530 2023-05-05 15:12:13.000000 PDFVisor-0.1.1/src/PDFViewr.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 17:56:52.000000 PDFVisor-0.1.1/src/__init__.py
+-rw-rw-rw-   0        0        0     4113 2023-04-14 20:56:10.000000 PDFVisor-0.1.1/src/funcsVisorPDF.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:23:52.978983 PDFVisor-0.1.1/src/img/
+-rw-rw-rw-   0        0        0     5315 2023-04-21 15:35:44.000000 PDFVisor-0.1.1/src/img/avanceDeshabilitado.png
+-rw-rw-rw-   0        0        0     4991 2023-04-21 14:52:58.000000 PDFVisor-0.1.1/src/img/avanceHighlight.png
+-rw-rw-rw-   0        0        0     4385 2023-04-21 15:23:16.000000 PDFVisor-0.1.1/src/img/avanceHighlightPressed.png
+-rw-rw-rw-   0        0        0     5250 2023-04-20 10:47:56.000000 PDFVisor-0.1.1/src/img/avanceNormal.png
+-rw-rw-rw-   0        0        0     5231 2023-04-21 15:37:12.000000 PDFVisor-0.1.1/src/img/retroDeshabilitado.png
+-rw-rw-rw-   0        0        0     4836 2023-04-21 15:27:38.000000 PDFVisor-0.1.1/src/img/retroHighlight.png
+-rw-rw-rw-   0        0        0     4305 2023-04-21 15:24:26.000000 PDFVisor-0.1.1/src/img/retroHighlightPressed.png
+-rw-rw-rw-   0        0        0     5947 2023-04-20 17:09:38.000000 PDFVisor-0.1.1/src/img/retroNormal.png
+-rw-rw-rw-   0        0        0  1206884 2022-05-07 05:19:20.000000 PDFVisor-0.1.1/src/times.ttf
```

### Comparing `PDFVisor-0.1.0/LICENSE.rst` & `PDFVisor-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.0/PDFVisor.egg-info/PKG-INFO` & `PDFVisor-0.1.1/PDFVisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDFVisor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Recurso para moverse por documentos PDF
 Author: Antonio San Román
 Author-email: asanro46@gmail.com
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
```

### Comparing `PDFVisor-0.1.0/PKG-INFO` & `PDFVisor-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDFVisor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Recurso para moverse por documentos PDF
 Author: Antonio San Román
 Author-email: asanro46@gmail.com
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
```

### Comparing `PDFVisor-0.1.0/README.md` & `PDFVisor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.0/setup.py` & `PDFVisor-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,51 +3,51 @@
 
 from setuptools import setup
 from distutils.command.register import register as register_orig
 from distutils.command.upload import upload as upload_orig
 
 
 HERE = pathlib.Path(__file__).parent
-ruta_paquete = "PDFVisor/src/img/*.png"
-relImags = os.path.relpath(ruta_paquete, r"img/*.png")
+#ruta_paquete = "PDFVisor/src/img/*.png"
+#relImags = os.path.relpath(ruta_paquete, r"img/*.png")
 
 class register(register_orig):
 
     def _get_rc_file(self):
         return os.path.join('.', '.pypirc')
 
 class upload(upload_orig):
 
-    def _get_rc_file(self):
+    def _get_rc_file(self):#
         return os.path.join('.', '.pypirc')
 
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
       "PyPDF2",
       "Pillow",
       "numpy",
       "PyMuPDF",
       "opencv-contrib-python",
       ] 
 
 setup(
     name= "PDFVisor",
-    version= '0.1.0',
+    version= '0.1.1',
     description= 'Recurso para moverse por documentos PDF',
     long_description=  (HERE / "README.md").read_text(encoding='utf-8'),
     long_description_content_type= "text/markdown",
     author= 'Antonio San Román',
     author_email= 'asanro46@gmail.com',
     install_requires=INSTALL_REQUIRES,
     license= 'MIT',
     packages= ['PDFVisor'],
     package_dir= {'PDFVisor': 'src'},
     package_data = {
-        'PDFVisor': ['funcsVisorPDF.py', '*README.md', relImags],
+        'PDFVisor': ['funcsVisorPDF.py', '*README.md', "LICENSE.rst", "MANIFEST.in"]
     },
     include_package_data=True,
     python_requires='>=3.4',
     cmdclass={
          'register': register,
          'upload': upload
          }
```

### Comparing `PDFVisor-0.1.0/src/PDFViewr.py` & `PDFVisor-0.1.1/src/PDFViewr.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,33 @@
    import tkinter as tk
    from tkinter.messagebox import showerror, showinfo
    import tkinter as tk
    from tkinter import ttk
    from tkinter import*
    import cv2
    import numpy as np
-   from PIL import Image, ImageTk 
+   from PIL import Image, ImageTk, ImageFont 
    import PDFVisor.funcsVisorPDF as vPDF
 except Exception as e:
       print(f"This error occured while importing neccesary modules or library {e}")   
 
 nombre = ""
 lenguaje = ""
 bandaFrame = None
 marcovisor = None
 opcion = ""
 image_on_canvas = None
 
+def centraTexto(text, font_size, centroFrame):
+    text = text[0:int(text.__len__()/2)]
+    fuente = ImageFont.truetype("times.ttf", font_size)
+    size = int(fuente.getlength(text))
+    return (centroFrame - size) - 47
+
+
 class Visor(tk.Frame):
      def __init__(self, master=None):
          #tk.Toplevel.__init__(self, master)
          tk.Frame.__init__(self, master)
          global btnEstado
          global bandaFrame
          global marcovisor
@@ -38,66 +45,66 @@
                                 [('Label.border',  {'sticky': 'nswe', 'border': '0',
                                   'children': [('Label.padding', {'sticky': 'nswe', 'border': '0',
                                   'children': [('Label.label', {'sticky': 'nswe'})]
                                  })]
                               }
                            )])
 
+     
          pdf_location = self.master.getvar(name="PDFDOC")
          auto = self
 
-         self.master.configure(height=820, width= 690, bg= "#1a5e92")
+         self.master.configure(height=675, width= 770, bg= "#1a5e92")
          #self.config(height=529, width= 330, bg= "#1a5e92")
-         self.grid_rowconfigure(0, weight= 80)
-         self.grid_rowconfigure(1, weight= 140)
+         self.grid_rowconfigure(0, weight= 60)
+         self.grid_rowconfigure(1, weight= 120)
          self.place()
          
-         bandaFrame = tk.Frame(self.master, bg="#2596be", height=80, width= 690)
-         bandaFrame.grid(row= 0, column= 0, padx=2, sticky="sw")
+         bandaFrame = tk.Frame(self.master, bg="#2596be", anchor= "NW", height=80, width= 770)
+         bandaFrame.grid(row= 0, column= 0, padx=2, sticky="nw")
          bandaFrame.grid_columnconfigure(0, weight=50)
          bandaFrame.grid_columnconfigure(1, weight=150)
          bandaFrame.grid_columnconfigure(2, weight=50)
-         bandaFrame.place()
+         bandaFrame.place_configure(x=0, y=0)
 
+         vPDF.desglosaPDF(self.master.getvar(name="PDFDOC"))
+         nomFile = self.master.getvar(name="PDFDOC")
+         nomFile = nomFile[0:-4] + "_Page-0.jpg"
+         img = Image.open(nomFile)
+         img = img.resize((770,605), Image.ANTIALIAS)
+         imgk = ImageTk.PhotoImage(img)
+         visorPDF = tk.Label(self.master, image= imgk, width=770, height=605, borderwidth= 6, bg= "white")
+         visorPDF.grid(row=0, column= 0, ipadx= 2, ipady=2, sticky= "sw")
+         visorPDF.place_configure(x=0, y=85, bordermode="outside")
+        
          btnEstado = vPDF.defEstado(self.master.getvar(name="PDFDOC"))
          archEstados = btnEstado["imagStates"]
          estados = btnEstado["Estado"]
          self.imgAvance = ImageTk.PhotoImage(file= r"./img/avanceNormal.png")
-         btnAvance = ttk.Label(bandaFrame, image= self.imgAvance, state= estados[0], width= 106, border=0)
+         btnAvance = ttk.Label(bandaFrame, image= self.imgAvance, state= estados[0], width= 106, border=0, background=None)
          btnAvance.config(style= "Emergency.TLabel")
-         btnAvance.grid(row=0, column=0, ipadx=0, ipady=0)
+         btnAvance.grid(row=0, column=0, ipadx=2, ipady=2)
          btnAvance.place()
 
          metaDataDoc = vPDF.metaDataPDF(self.master.getvar(name="PDFDOC"))
          rotulo = Canvas(bandaFrame, width=330, height=60, highlightthickness=0, bg="#2596be", bd=0, borderwidth= 0)
-         rotulo.grid(row=0, column=1, ipady=0)
+         rotulo.grid(row=0, column=1, ipady=0, ipadx=5)
          metadatosPDF = "{}\n{}".format(metaDataDoc.get("Titulo"), metaDataDoc.get("Fecha_creacion"))
-         lblInformacion = rotulo.create_text(95, 30, justify="center", text= metadatosPDF, fill="white", font= ("Times New Roman", 12, "bold"))
+         x = centraTexto(metaDataDoc.get("Titulo"), 12, int(bandaFrame.cget('width')/2))
+         lblInformacion = rotulo.create_text(x, 30, justify="center", text= metadatosPDF, fill="white", font= ("Times New Roman", 12, "bold"))
 
          btnEstado = vPDF.defEstado(self.master.getvar(name="PDFDOC"))
          archEstados = btnEstado["imagStates"]  #estados[1]
          estados = btnEstado["Estado"]
          self.imgRetro = ImageTk.PhotoImage(file= archEstados[1]) 
          btnRetro = ttk.Label(bandaFrame, image= self.imgRetro, state= "normal", width= 106)  
          btnRetro.config(style= "Emergency.TLabel")
          btnRetro.grid(row=0, column=2)
          btnRetro.place()
 
-         vPDF.desglosaPDF(self.master.getvar(name="PDFDOC"))        
-         marcovisor = tk.Frame(bandaFrame, width= 50, height= 620, borderwidth= 3, bg= "#2596be", relief= "raised")
-         marcovisor.grid(row=1, column=0, padx= 2, pady= 2, sticky="se")
-         marcovisor.place()
-         visorPDF = Canvas(marcovisor, width=835, height=605, borderwidth= 0, bg= "white")
-         visorPDF.grid(row=0, column= 0, padx= 2, pady=2, sticky= "nw")
-         visorPDF.place()
-         self.imgk = ImageTk.PhotoImage(file= r"D:/Temp/PARREL-ISEC(Feb 23)_Page-0.jpg")
-         image_on_canvas = visorPDF.create_image(1, 1, image= self.imgk, anchor= tk.NW, )
- 
-         print(marcovisor.children['!canvas'])
-         
          vPDF.grid_by_column(bandaFrame, 3)
          
          self.gestorEventos()
 
      def on_enter(self, parOpcion, opcion, fileflecha):
          global btnEstado
```

### Comparing `PDFVisor-0.1.0/src/funcsVisorPDF.py` & `PDFVisor-0.1.1/src/funcsVisorPDF.py`

 * *Files identical despite different names*

