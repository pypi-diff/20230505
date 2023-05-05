# Comparing `tmp/blctools-0.0.8.tar.gz` & `tmp/blctools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blctools-0.0.8.tar", last modified: Sat Sep 17 19:02:20 2022, max compression
+gzip compressed data, was "blctools-0.0.9.tar", last modified: Tue Sep 20 10:40:49 2022, max compression
```

## Comparing `blctools-0.0.8.tar` & `blctools-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-09-17 19:02:20.764479 blctools-0.0.8/
--rw-rw-rw-   0        0        0     1091 2022-06-12 22:36:58.000000 blctools-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1168 2022-09-17 19:02:20.765479 blctools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      597 2022-09-17 18:59:19.000000 blctools-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-09-17 19:02:20.731502 blctools-0.0.8/blctools/
--rw-rw-rw-   0        0        0     1073 2022-09-17 18:58:58.000000 blctools-0.0.8/blctools/__init__.py
--rw-rw-rw-   0        0        0    10655 2022-09-16 20:20:07.000000 blctools-0.0.8/blctools/cl_ApiCammesa.py
--rw-rw-rw-   0        0        0     2540 2022-06-16 18:05:48.000000 blctools-0.0.8/blctools/cl_CarpetaServicios.py
--rw-rw-rw-   0        0        0     2827 2022-07-12 11:44:48.000000 blctools-0.0.8/blctools/cl_DTE.py
--rw-rw-rw-   0        0        0    55322 2022-09-16 20:10:52.000000 blctools-0.0.8/blctools/cl_DatosCROM.py
--rw-rw-rw-   0        0        0     2771 2022-06-16 18:06:17.000000 blctools-0.0.8/blctools/cl_PPO.py
--rw-rw-rw-   0        0        0     5934 2022-06-28 15:03:42.000000 blctools-0.0.8/blctools/cl_Pronosticos.py
--rw-rw-rw-   0        0        0    18242 2022-07-12 12:31:14.000000 blctools-0.0.8/blctools/cl_ReporteBase.py
--rw-rw-rw-   0        0        0    29424 2022-09-07 17:11:47.000000 blctools-0.0.8/blctools/cl_TablasVC.py
--rw-rw-rw-   0        0        0     2890 2022-06-15 18:17:12.000000 blctools-0.0.8/blctools/cl_UsuarioCammesa.py
--rw-rw-rw-   0        0        0     5299 2022-06-30 20:05:04.000000 blctools-0.0.8/blctools/dirs.py
--rw-rw-rw-   0        0        0     1579 2022-09-12 18:56:53.000000 blctools-0.0.8/blctools/eo.py
--rw-rw-rw-   0        0        0     5724 2022-06-29 00:35:58.000000 blctools-0.0.8/blctools/fechas.py
--rw-rw-rw-   0        0        0        0 2022-06-11 20:16:09.000000 blctools-0.0.8/blctools/fv.py
-drwxrwxrwx   0        0        0        0 2022-09-17 19:02:20.763481 blctools-0.0.8/blctools.egg-info/
--rw-rw-rw-   0        0        0     1168 2022-09-17 19:02:20.000000 blctools-0.0.8/blctools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2022-09-17 19:02:20.000000 blctools-0.0.8/blctools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-17 19:02:20.000000 blctools-0.0.8/blctools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-09-17 19:02:20.000000 blctools-0.0.8/blctools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-09-17 19:02:20.000000 blctools-0.0.8/blctools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-06-12 23:25:33.000000 blctools-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      707 2022-09-17 19:02:20.773474 blctools-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-09-20 10:40:49.698081 blctools-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2022-06-12 22:36:58.000000 blctools-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1429 2022-09-20 10:40:49.700076 blctools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2022-09-19 11:37:35.000000 blctools-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-09-20 10:40:49.654104 blctools-0.0.9/blctools/
+-rw-rw-rw-   0        0        0     1073 2022-09-17 19:15:17.000000 blctools-0.0.9/blctools/__init__.py
+-rw-rw-rw-   0        0        0    10655 2022-09-16 20:20:07.000000 blctools-0.0.9/blctools/cl_ApiCammesa.py
+-rw-rw-rw-   0        0        0     2462 2022-09-17 19:49:17.000000 blctools-0.0.9/blctools/cl_CarpetaServicios.py
+-rw-rw-rw-   0        0        0     2778 2022-09-17 19:49:16.000000 blctools-0.0.9/blctools/cl_DTE.py
+-rw-rw-rw-   0        0        0    55852 2022-09-20 10:36:51.000000 blctools-0.0.9/blctools/cl_DatosCROM.py
+-rw-rw-rw-   0        0        0     2769 2022-09-17 19:49:27.000000 blctools-0.0.9/blctools/cl_PPO.py
+-rw-rw-rw-   0        0        0     5934 2022-06-28 15:03:42.000000 blctools-0.0.9/blctools/cl_Pronosticos.py
+-rw-rw-rw-   0        0        0    17716 2022-09-17 20:35:50.000000 blctools-0.0.9/blctools/cl_ReporteBase.py
+-rw-rw-rw-   0        0        0    29424 2022-09-19 11:18:42.000000 blctools-0.0.9/blctools/cl_TablasVC.py
+-rw-rw-rw-   0        0        0     2890 2022-06-15 18:17:12.000000 blctools-0.0.9/blctools/cl_UsuarioCammesa.py
+-rw-rw-rw-   0        0        0     5299 2022-09-19 11:23:12.000000 blctools-0.0.9/blctools/dirs.py
+-rw-rw-rw-   0        0        0     1579 2022-09-12 18:56:53.000000 blctools-0.0.9/blctools/eo.py
+-rw-rw-rw-   0        0        0     5724 2022-06-29 00:35:58.000000 blctools-0.0.9/blctools/fechas.py
+-rw-rw-rw-   0        0        0        0 2022-06-11 20:16:09.000000 blctools-0.0.9/blctools/fv.py
+drwxrwxrwx   0        0        0        0 2022-09-20 10:40:49.693081 blctools-0.0.9/blctools.egg-info/
+-rw-rw-rw-   0        0        0     1429 2022-09-20 10:40:49.000000 blctools-0.0.9/blctools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2022-09-20 10:40:49.000000 blctools-0.0.9/blctools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-20 10:40:49.000000 blctools-0.0.9/blctools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2022-09-20 10:40:49.000000 blctools-0.0.9/blctools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-06-12 23:25:33.000000 blctools-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      647 2022-09-20 10:40:49.714071 blctools-0.0.9/setup.cfg
```

### Comparing `blctools-0.0.8/LICENSE` & `blctools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blctools-0.0.8/PKG-INFO` & `blctools-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blctools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools to work with data inside BLCs MS Sharepoint Cloud & Database
 Home-page: https://github.com/DiegoRioboCabot/blctools
 Author: Diego Riobo Cabot
 Author-email: riobocabotd@gmail.com
 Project-URL: Bug Tracker, https://github.com/DiegoRioboCabot/blctools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,28 +13,31 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BLC Data Analytics tools package
 
 Data Analytics helper functions to work with inside BLC's Cloud system.
 
-
-
 # Changelog
 ## Version 0.0.1
- Basic functionality is up and running
+* Basic functionality is up and running
 
 ## Version 0.0.2 ~ 0.0.4
 Fixed the install issues
 
 ## Version 0.0.5
 * Most of the code is Object Oriented now.
 * CAMMESA's forecasts have been added.
 
 ## Version 0.0.6 ~ 0.0.7
 * Bug fixes regarding file management
 * Ability to customize filters when hitting CAMMESA's API
 * PBA calculation according to IEC61400 is still functioning incorrectly
 
-
 ## Version 0.0.8
 * Corrected dependencies list
+
+## Version 0.0.9
+* Removed dependencies list
+* Ability to download unfiltered PPOs/DTEs without specifying parks/plants list
+* Incidents are no longer loaded by default on blctools.DatosCrom() objects
+* TO DO: Use SQLAlchemy to retrieve SQL data with pandas.
```

### Comparing `blctools-0.0.8/blctools/__init__.py` & `blctools-0.0.9/blctools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 from .cl_PPO import *               # Derivada de la clase cl_ReporteBase. Simplemente tiene configuraciones "listas para" consultar los reportes PPO diarios de CAMMESA
 from .cl_DTE import *               # Derivada de la clase cl_ReporteBase. Simplemente tiene configuraciones "listas para" consultar los reportes DTE mensuales de CAMMESA
 
 from .cl_TablasVC import *
 from .cl_DatosCROM import *
 
 #Versión
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

### Comparing `blctools-0.0.8/blctools/cl_ApiCammesa.py` & `blctools-0.0.9/blctools/cl_ApiCammesa.py`

 * *Files identical despite different names*

### Comparing `blctools-0.0.8/blctools/cl_CarpetaServicios.py` & `blctools-0.0.9/blctools/cl_CarpetaServicios.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 
 __all__ = ['__CarpetaServicios']
 
 
 mensaje = """No se ha encontrado la carpeta hacia la nube de BLC.\n
 Tendrá que indicar la ruta hacia la carpeta de Servicios manualmente.
-Para ello por favor ejecutar el comando: blctools.indicar_ruta('ruta compl
-
-eta')
+Para ello por favor ejecutar el comando: blctools.indicar_ruta('ruta completa')
 Mientras tanto se trabajará en la ruta del script actual"""
 
 
 class __CarpetaServicios():
        
     def __init__(self):
         self._ruta = str(Path.cwd())
@@ -24,15 +22,14 @@
             try: 
                 self.__buscar_dir_segun_archivo_py()
             except:
                 self.print_warning
         
     def __buscar_dir_segun_archivo_py(self):
         if r'Documentos Produccion\Servicios' in self.ruta:
-            print('Ingresó al método de búsqueda según archivo .py')
             dir_raiz_split = self.ruta.split('\\')
             index_dir_servicios = dir_raiz_split.index('Servicios')
             dir_servicios = '\\'.join(dir_raiz_split[0:index_dir_servicios+1])
             
             self.ruta = dir_servicios
             self.ruta_encontrada = True
```

### Comparing `blctools-0.0.8/blctools/cl_DTE.py` & `blctools-0.0.9/blctools/cl_DTE.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-from blctools.cl_ApiCammesa import ApiCammesa
 from . import dirs
 from . import fechas
 
 from .cl_ReporteBase import *
 
 __all__ = ['DTE',]
```

### Comparing `blctools-0.0.8/blctools/cl_DatosCROM.py` & `blctools-0.0.9/blctools/cl_DatosCROM.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,39 +17,44 @@
     def __init__(
         self,
         fecha_i = None,
         fecha_f = None,
         parques = [],
         clientes = [],
         dir_salida = None,
-        cargar_incidencias=True,
+        cargar_incidencias=False,
         cargar_datos_segundales=False,
         cargar_instancia=None
         ):
         
-        
         initialize = True
         
-        if not cargar_instancia is None:
-            if isinstance(cargar_instancia,Path):
-                archivo = cargar_instancia.resolve()
-            elif isinstance(cargar_instancia,str):
-                archivo = Path(cargar_instancia).resolve()
-            else:
-                raise TypeError('Cargar instancia debe ser un objeto pathlib.Path o una ruta a un archivo .pickle en formato string')
-            
-            if cargar_instancia.suffix != '.pickle':
-                raise ValueError('La ruta al archivo de instancia debe ser en formato .pickle')
-            else:
-                try:
-                    #self.load(str(archivo))
-                    #initialize = False
-                    pass
-                except:
-                    pass
+        # Esto todavía no está resuelto.
+        #la idea es que, con necesidades del testing, se puedan cargar objetos y guardar su estado
+        # luego, crear nuevos objetos, pero retomar desde un estado anterior, guardado en un archivo.
+        # Bastante complicado, ya que no es lo mismo "la instancia de un objeto" que "los datos que contiene"
+        # Decidir qué hacer
+        
+        # if not cargar_instancia is None:
+        #     if isinstance(cargar_instancia,Path):
+        #         archivo = cargar_instancia.resolve()
+        #     elif isinstance(cargar_instancia,str):
+        #         archivo = Path(cargar_instancia).resolve()
+        #     else:
+        #         raise TypeError('Cargar instancia debe ser un objeto pathlib.Path o una ruta a un archivo .pickle en formato string')
+            
+        #     if cargar_instancia.suffix != '.pickle':
+        #         raise ValueError('La ruta al archivo de instancia debe ser en formato .pickle')
+        #     else:
+        #         try:
+        #             #self.load(str(archivo))
+        #             #initialize = False
+        #             pass
+        #         except:
+        #             pass
 
         if initialize:
             self.init_sequence(
                 fecha_i = fecha_i,
                 fecha_f = fecha_f,
                 parques = parques,
                 clientes = clientes,
@@ -938,51 +943,50 @@
             else:
                 col_prioridad = f'Priority_{metodo}'
 
 
         parques_con_datos = self.datos_seg.index.levels[0]
         
         for parque in parques_con_datos:
+            print(f'Roll Down de incidencias: {parque}')
+            
+            parque_selec = (parque,slice(None))
             plant_selec = ('PLANT',cols_por_incidencia)
             plant_prioridad = ('PLANT',col_prioridad)
-            flt_tiene_inci_plant = self._rpt_consolidado_seg.loc[:,plant_prioridad] > 1
             
-            
-            print('Iniciando Roll Down de incidencias...')
-            print(f'Parque {parque}')
+            flt_tiene_inci_plant = self._rpt_consolidado_seg.loc[parque_selec,plant_prioridad] > 1
+
             agrupamientos = self.consultar_equipos_por_agrupamiento(nemo_parque=parque) 
             for agrup,equipos_asociados in agrupamientos.items():
                 agrup_selec = (agrup,cols_por_incidencia)
                 agrup_prioridad = (agrup,col_prioridad)
-                flt_tiene_inci_agrup = self._rpt_consolidado_seg.loc[:,agrup_prioridad] > 1
+                flt_tiene_inci_agrup = self._rpt_consolidado_seg.loc[parque_selec,agrup_prioridad] > 1
                 
                 for equipo in equipos_asociados:
-                    print(f'Equipo: {equipo}')
+                    print(f'Roll Down de incidencias: {parque} {equipo}. Buscando Incidencias...')
                     equipo_selec = (equipo,cols_por_incidencia)
                     equipo_prioridad = (equipo,col_prioridad)
-                    flt_tiene_inci_equipo = self._rpt_consolidado_seg.loc[:,equipo_prioridad] > 1
+                    flt_tiene_inci_equipo = self._rpt_consolidado_seg.loc[parque_selec,equipo_prioridad] > 1
                     
                     flt = flt_tiene_inci_plant | flt_tiene_inci_agrup | flt_tiene_inci_equipo
                     
                     j = None
                     for i in self._rpt_consolidado_seg.loc[flt,:].index:
                         if j != i[1].date():
                             j = i[1].date()
-                            print(f'Equipo {equipo} Fecha {j}')
+                            print(f'Roll Down de incidencias: {parque} {equipo} {j}. Procesando')
                             
-                            if self._rpt_consolidado_seg.loc[[i],[plant_prioridad]].iat[0,0] > self._rpt_consolidado_seg.loc[[i],[agrup_prioridad]].iat[0,0]:
-                                self._rpt_consolidado_seg.loc[i,agrup_selec] = self._rpt_consolidado_seg.loc[i,plant_selec]
+                        if self._rpt_consolidado_seg.loc[[i],[plant_prioridad]].iat[0,0] > self._rpt_consolidado_seg.loc[[i],[agrup_prioridad]].iat[0,0]:
+                            self._rpt_consolidado_seg.loc[i,agrup_selec] = self._rpt_consolidado_seg.loc[i,plant_selec]
 
-                                if self._rpt_consolidado_seg.loc[[i],[equipo_prioridad]].iat[0,0] > self._rpt_consolidado_seg.loc[[i],[agrup_prioridad]].iat[0,0]:
-                                    self._rpt_consolidado_seg.loc[i,equipo_selec] = self._rpt_consolidado_seg.loc[i,agrup_selec]
+                            if self._rpt_consolidado_seg.loc[[i],[equipo_prioridad]].iat[0,0] > self._rpt_consolidado_seg.loc[[i],[agrup_prioridad]].iat[0,0]:
+                                self._rpt_consolidado_seg.loc[i,equipo_selec] = self._rpt_consolidado_seg.loc[i,agrup_selec]
         print('Listo!')                
 
 
-
-
     def reporte_iec61400(self,metodo='WTG',granularidades=['1D','1M'],ruta=None,nombre=None):
         
         self.__rolldown_incidencias(metodo=metodo)
         
         indisponibilidad_TBA = ['MAPRO','MANOPRO','MAPRO S_A','FAILURE']
         parques_con_datos = self.datos_seg.index.levels[0]
```

### Comparing `blctools-0.0.8/blctools/cl_PPO.py` & `blctools-0.0.9/blctools/cl_PPO.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from . import dirs
 from . import fechas
 
 from .cl_ReporteBase import *
 
 __all__ = ['PPO',]
```

### Comparing `blctools-0.0.8/blctools/cl_Pronosticos.py` & `blctools-0.0.9/blctools/cl_Pronosticos.py`

 * *Files identical despite different names*

### Comparing `blctools-0.0.8/blctools/cl_ReporteBase.py` & `blctools-0.0.9/blctools/cl_ReporteBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -363,17 +363,21 @@
 
     def _procesar_archivos(self):
         '''Abre y filtra todos los archivos disponibles MDB para los parques seleccionados.
         Devuelve un df de pandas unificado.
         '''
         driver = '{Microsoft Access Driver (*.mdb, *.accdb)}'
         
-        lista_sql = self.__get_lista_sql()
+        if self.parques:
+            lista_sql = self.__get_lista_sql()
 
-        SQL_datos = f'SELECT * FROM {self.tabla_datos} WHERE {self.col_filtro} IN {lista_sql};'
+            SQL_datos = f'SELECT * FROM {self.tabla_datos} WHERE {self.col_filtro} IN {lista_sql};'
+        else:
+            SQL_datos = f'SELECT * FROM {self.tabla_datos};'
+            
         SQL_fecha = f'SELECT * FROM {self.tabla_fecha};'
 
         data_total = []
         encabezados = []
 
         for archivo in self.archivos_disponibles:
             print(f'Cargando .mdb en la memoria: {archivo.name}')
@@ -436,23 +440,14 @@
 
     def cargar(self,descargar=False,filtro=False):
         '''Función que realiza la consulta en CAMMESA por en un rango de fechas, descarga los archivos .zip,
         extrae los archivos .mdb dentro de los archivos .zip, 
         filtra la tabla del archivo MDB seleccionada según el listado de parques provisto
         la columna provista y devuelve el resultado como un dataframe de pandas
         '''
-
-        # Acá hay que agregar una función que cree filtros custom, para poder bajar los rpts iniciales y los finales estrictamente
-        # La ApiCammesa permite distinguir entre "los primeros" y "los ultimos". 
-        # Los primeros siempre serán la versión inicial. Pero "los últimos" no necesariamente son la versión final de cada documento
-
-        #Para tal fin, habría que hacer una consulta a la api, y filtrar el df de consulta desde aquí
-        #Ya que la función descarga, toma el atributo self.consulta como input
-
-        #Pasando filtro como true, se baja el self._consulta_custom, que se debe modificar desde aquí
         
         if descargar == True:
             self.descargar(
                 exportar_consulta=False,
                 dir_consulta=None, 
                 filtro=filtro
             )
```

### Comparing `blctools-0.0.8/blctools/cl_TablasVC.py` & `blctools-0.0.9/blctools/cl_TablasVC.py`

 * *Files identical despite different names*

### Comparing `blctools-0.0.8/blctools/cl_UsuarioCammesa.py` & `blctools-0.0.9/blctools/cl_UsuarioCammesa.py`

 * *Files identical despite different names*

### Comparing `blctools-0.0.8/blctools/dirs.py` & `blctools-0.0.9/blctools/dirs.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,20 +47,20 @@
     '''Devuelve la ruta a la carpeta de DTES Iniciales en la carpeta de datos crudos de AM'''
     
     return get_dc_cammesa() + '\\03 DTE I'
 
 def get_dc_dtef():
     '''Devuelve la ruta a la carpeta de DTES Iniciales en la carpeta de datos crudos de AM'''
     
-    return get_dc_cammesa() + '\\04 DTE F'
+    return get_dc_cammesa() + '\\03 DTE F'
 
 def get_dc_dte():
     '''Devuelve la ruta a la carpeta de DTES Iniciales en la carpeta de datos crudos de AM'''
     
-    return get_dc_cammesa() + '\\09 DTE UNIF'
+    return get_dc_cammesa() + '\\03 DTE UNIF'
 
 def get_dc_pronosticos():
     '''Devuelve la ruta a la carpeta de DTES Iniciales en la carpeta de datos crudos de AM'''
     
     return get_dc_cammesa() + '\\05 PRONOSTICOS'
 
 def get_dc_10s():
```

### Comparing `blctools-0.0.8/blctools/eo.py` & `blctools-0.0.9/blctools/eo.py`

 * *Files identical despite different names*

### Comparing `blctools-0.0.8/blctools/fechas.py` & `blctools-0.0.9/blctools/fechas.py`

 * *Files identical despite different names*

### Comparing `blctools-0.0.8/blctools.egg-info/PKG-INFO` & `blctools-0.0.9/blctools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blctools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools to work with data inside BLCs MS Sharepoint Cloud & Database
 Home-page: https://github.com/DiegoRioboCabot/blctools
 Author: Diego Riobo Cabot
 Author-email: riobocabotd@gmail.com
 Project-URL: Bug Tracker, https://github.com/DiegoRioboCabot/blctools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,28 +13,31 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BLC Data Analytics tools package
 
 Data Analytics helper functions to work with inside BLC's Cloud system.
 
-
-
 # Changelog
 ## Version 0.0.1
- Basic functionality is up and running
+* Basic functionality is up and running
 
 ## Version 0.0.2 ~ 0.0.4
 Fixed the install issues
 
 ## Version 0.0.5
 * Most of the code is Object Oriented now.
 * CAMMESA's forecasts have been added.
 
 ## Version 0.0.6 ~ 0.0.7
 * Bug fixes regarding file management
 * Ability to customize filters when hitting CAMMESA's API
 * PBA calculation according to IEC61400 is still functioning incorrectly
 
-
 ## Version 0.0.8
 * Corrected dependencies list
+
+## Version 0.0.9
+* Removed dependencies list
+* Ability to download unfiltered PPOs/DTEs without specifying parks/plants list
+* Incidents are no longer loaded by default on blctools.DatosCrom() objects
+* TO DO: Use SQLAlchemy to retrieve SQL data with pandas.
```

### Comparing `blctools-0.0.8/setup.cfg` & `blctools-0.0.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6c63 746f 6f6c 730d 0a76 6572   = blctools..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000030: 7468 6f72 203d 2044 6965 676f 2052 696f  thor = Diego Rio
 00000040: 626f 2043 6162 6f74 0d0a 6175 7468 6f72  bo Cabot..author
 00000050: 5f65 6d61 696c 203d 2072 696f 626f 6361  _email = rioboca
 00000060: 626f 7464 4067 6d61 696c 2e63 6f6d 0d0a  botd@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 546f  description = To
 00000080: 6f6c 7320 746f 2077 6f72 6b20 7769 7468  ols to work with
 00000090: 2064 6174 6120 696e 7369 6465 2042 4c43   data inside BLC
@@ -31,15 +31,11 @@
 000001e0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
 000001f0: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
 00000200: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
 00000210: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
 00000220: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
 00000230: 6b61 6765 7320 3d20 626c 6374 6f6f 6c73  kages = blctools
 00000240: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-00000250: 7320 3d20 3e3d 332e 360d 0a69 6e73 7461  s = >=3.6..insta
-00000260: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000270: 0970 796f 6462 630d 0a09 7061 6e64 6173  .pyodbc...pandas
-00000280: 0d0a 0970 796d 7973 716c 0d0a 0972 6571  ...pymysql...req
-00000290: 7565 7374 730d 0a0d 0a5b 6567 675f 696e  uests....[egg_in
-000002a0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000002b0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000002c0: 0a0d 0a                                  ...
+00000250: 7320 3d20 3e3d 332e 360d 0a0d 0a5b 6567  s = >=3.6....[eg
+00000260: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000270: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000280: 3d20 300d 0a0d 0a                        = 0....
```

