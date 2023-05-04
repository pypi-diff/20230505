# Comparing `tmp/pih-1.421.tar.gz` & `tmp/pih-1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.421.tar", last modified: Wed Mar 29 00:11:00 2023, max compression
+gzip compressed data, was "pih-1.43.tar", last modified: Thu May  4 23:32:40 2023, max compression
```

## Comparing `pih-1.421.tar` & `pih-1.43.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 00:10:56.709822 pih-1.421/
--rw-rw-rw-   0        0        0      259 2023-03-29 00:11:01.032021 pih-1.421/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-29 00:10:59.912768 pih-1.421/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.421/pih/__init__.py
--rw-rw-rw-   0        0        0    13100 2023-03-28 05:49:41.000000 pih-1.421/pih/collection.py
--rw-rw-rw-   0        0        0    42394 2023-03-28 23:10:25.000000 pih-1.421/pih/console_api.py
--rw-rw-rw-   0        0        0    81562 2023-03-29 00:09:52.000000 pih-1.421/pih/const.py
--rw-rw-rw-   0        0        0   211422 2023-03-29 00:10:25.000000 pih-1.421/pih/pih.py
--rw-rw-rw-   0        0        0    15235 2023-03-20 04:28:02.000000 pih-1.421/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.421/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.421/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      557 2022-11-27 04:03:58.000000 pih-1.421/pih/rpc_collection.py
--rw-rw-rw-   0        0        0    28573 2023-03-28 05:49:08.000000 pih-1.421/pih/tools.py
--rw-rw-rw-   0        0        0     2037 2022-10-21 06:31:07.000000 pih-1.421/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-03-29 00:11:00.922636 pih-1.421/pih.egg-info/
--rw-rw-rw-   0        0        0      259 2023-03-29 00:10:54.000000 pih-1.421/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-03-29 00:10:56.000000 pih-1.421/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 00:10:54.000000 pih-1.421/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-03-29 00:10:55.000000 pih-1.421/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-29 00:10:55.000000 pih-1.421/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2090 2023-03-22 01:39:03.000000 pih-1.421/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-03-29 00:11:01.047636 pih-1.421/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 23:32:40.314156 pih-1.43/
+-rw-rw-rw-   0        0        0      258 2023-05-04 23:32:40.298564 pih-1.43/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 23:32:39.423602 pih-1.43/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.43/pih/__init__.py
+-rw-rw-rw-   0        0        0    15492 2023-05-02 07:21:58.000000 pih-1.43/pih/collection.py
+-rw-rw-rw-   0        0        0    49882 2023-04-26 06:39:23.000000 pih-1.43/pih/console_api.py
+-rw-rw-rw-   0        0        0    92125 2023-05-04 23:30:36.000000 pih-1.43/pih/const.py
+-rw-rw-rw-   0        0        0   239867 2023-05-04 23:31:39.000000 pih-1.43/pih/pih.py
+-rw-rw-rw-   0        0        0    19843 2023-05-04 23:27:46.000000 pih-1.43/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.43/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.43/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      624 2023-03-29 23:40:14.000000 pih-1.43/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0      793 2023-04-22 17:05:00.000000 pih-1.43/pih/service_example.py
+-rw-rw-rw-   0        0        0    29939 2023-05-04 01:10:38.000000 pih-1.43/pih/tools.py
+-rw-rw-rw-   0        0        0     2037 2022-10-21 06:31:07.000000 pih-1.43/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-04 23:32:40.079778 pih-1.43/pih.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-05-04 23:32:36.000000 pih-1.43/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-04 23:32:37.000000 pih-1.43/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 23:32:36.000000 pih-1.43/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-04 23:32:36.000000 pih-1.43/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-04 23:32:36.000000 pih-1.43/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2130 2023-05-04 23:29:46.000000 pih-1.43/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 23:32:40.345417 pih-1.43/setup.cfg
```

### Comparing `pih-1.421/pih/console_api.py` & `pih-1.43/pih/console_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+from typing import Any, Callable
 import importlib.util
 import sys
 from subprocess import CompletedProcess
-from typing import Any, List
+from typing import Any
+from datetime import datetime
+import os
 
 pih_is_exists = importlib.util.find_spec("pih.pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
-from pih import PIH, A, NotFound, ActionValue, ActionStack, Input, Output, Session
-from pih.tools import EnumTool, FullNameTool, ResultTool, DataTool, StringTool
-from pih.const import CONST, MarkType, PASSWORD, USER_PROPERTY, FIELD_COLLECTION, PasswordSettings, CheckableSections
-from pih.collection import Mark, User, FullName, MarkDivision, UserContainer, LoginPasswordPair, MarkGroup, Result, FieldItemList, WorkstationDescription, ResourceStatus, SiteResourceStatus, CTIndicationValue, CTIndicationDS
+from pih.const import CONST, MarkType, PASSWORD, USER_PROPERTY, FIELD_COLLECTION, PasswordSettings, CheckableSections, HOSTS, AD, PATHS, FILE
+from pih import PIH, A, NotFound, ActionValue, ActionStack, Input, Output, Session, while_not_do
+from pih.tools import EnumTool, FullNameTool, ResultTool, DataTool, StringTool, DateTimeTool, PathTool
+from pih.collection import Mark, User, FullName, MarkDivision, UserContainer, LoginPasswordPair, MarkGroup, Result, FieldItemList, WorkstationDescription, ResourceStatus, SiteResourceStatus, CTIndicationValue, Workstation, RobocopyJobStatus
+from pih import A
 
 class ConsoleAppsApi:
 
     LINE: str = "........................................................"
 
     def __init__(self, pih: PIH = None):
         self.pih = pih or PIH
@@ -30,55 +34,151 @@
         self.polibase_login: str = None
         self.polibase_password: str = None
         self.user_container: UserContainer
         self.description: str = None
         self.use_template_user: bool
         self.need_to_create_mark: bool = None
 
-    def check_resources_and_indications(self, checkable_section_list: List[CheckableSections], ask_for_update_before: bool = False, force_update: bool = False, all: bool = False) -> None:
+    def create_qr_code_for_mobile_helper_command(self, command: str | None = None, title: str | None = None, show_result: bool = True) -> str | None:
+        command = command or self.input.input("Введите название команды")
+        title = title or self.input.input("Введите заголовок")
+        result = A.A_QR.for_mobile_helper_command(command, title, os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(command, FILE.EXTENSION.PNG))), 56)
+        qr_code_image_path: str = A.PTH_QR.mobile_helper_command(command)
+        if show_result:
+            if result:
+                self.output.good(
+                    f"Файл qr кода {self.bold(title)} создан.\nПуть к файлу:\n{self.bold(qr_code_image_path)}\n")
+            else:
+                self.output.error("qr код не был создан")
+        return qr_code_image_path
+
+    def create_qr_code_for_card_registry_folder(self, card_registry_folder_name: str | None = None, show_result: bool = True) -> str | None:
+        card_registry_folder_name = A.D_F.polibase_person_card_registry_folder(card_registry_folder_name or self.input.input("Введите название папки")) 
+        result: bool = A.A_QR.for_polibase_person_card_registry_folder(card_registry_folder_name)
+        qr_code_image_path: str = PIH.PATH.QR_CODE.polibase_person_card_registry_folder(card_registry_folder_name)
+        if show_result:
+            if result:
+                self.output.good(
+                    f"Файл qr код для папки реестра карт пациентов {self.bold(card_registry_folder_name)} создан.\nПуть к файлу:\n{self.bold(qr_code_image_path)}\n")    
+            else:
+                self.output.error("qr код не был создан")
+        return qr_code_image_path if result else None
+
+    def resources_and_indications_check(self, checkable_section_list: list[CheckableSections], ask_for_update_before: bool = False, force_update: bool = False, all: bool = False) -> None:
         if CheckableSections.RESOURCES in checkable_section_list or CheckableSections.WS in checkable_section_list:
-            def label_function(resource: ResourceStatus) -> str:
-                result: list[str] = []
+            def label_function(resource: ResourceStatus, index: int) -> str:
+                result: list[str] = [] 
                 accessable: bool = resource.accessable
-                result.append(self.bold(self.output.blue_str(resource.name)) + ": " + (
-                    self.output.good_str("доступен") if accessable else self.bold(self.output.red_str("не доступен!"))))
+                status: str = self.output.good_str("доступен") if accessable else self.bold(
+                    self.output.red_str("не доступен!"))
+                result.append(self.bold(self.output.blue_str(
+                    resource.name)) + ("" if isinstance(resource, SiteResourceStatus) else f": {status}"))
                 if isinstance(resource, SiteResourceStatus):
                     if resource.check_free_space_status:
-                        free_space_result_list: str = resource.free_space_status.split(
-                            " ")
-                        result.append(self.output.black_str(
-                            f"Cвободное место: {free_space_result_list[0]} ({free_space_result_list[1]})"))
+                        free_space_result_list: str = resource.free_space_status.split(" ")
+                        result.append(f"Cвободное место: {free_space_result_list[0]} ({free_space_result_list[1]})")
                     if resource.check_certificate_status:
-                        result.append(self.output.black_str(
-                            f"Сертификат доступен до: {resource.certificate_status}"))
+                        result.append(f"Сертификат доступен до: {resource.certificate_status}")
+                    result.append(ConsoleAppsApi.LINE)
+                    result.append(status)
                 return "\n".join(result)
             force_update = force_update or (ask_for_update_before and self.input.yes_no(
                 "Обновить перед получением"))
             if force_update:
                 self.output.write_line(
                     self.italic(f"{self.get_formatted_given_name()}, ожидайте получение результата..."))
             for checkable_section in [CheckableSections.RESOURCES, CheckableSections.WS]:
-                self.output.new_line()
-                self.output.write_result(A.R_RM.get_status_list([checkable_section], force_update, all if len(checkable_section_list) == 1 and CheckableSections.WS in checkable_section_list else False), False, label_function=label_function, separated_result_item=True, title = (self.output.bold(CONST.VISUAL.BULLET + (" Основные ресурсы" if checkable_section == CheckableSections.RESOURCES else " Наблюдаемые компьютеры")) ) if all else None )
+                if checkable_section in checkable_section_list:
+                    self.output.new_line()
+                    self.output.write_result(A.R_R.get_status_list([checkable_section], force_update, all if len(checkable_section_list) == 1 and CheckableSections.WS in checkable_section_list else False), False, label_function=label_function, separated_result_item=True, title = (self.output.bold(CONST.VISUAL.BULLET + (" Основные ресурсы" if checkable_section == CheckableSections.RESOURCES else " Наблюдаемые компьютеры")) ) if all else None )
         if CheckableSections.INDICATIONS in checkable_section_list:
             self.output.new_line()
-            self.output.write_result(A.R_I.get_last_values(), title=self.output.bold((CONST.VISUAL.BULLET + " " if all else "") + "Показания в помещение КТ"))
+            self.output.write_result(A.R_I.get_last_items(), title=self.output.bold((CONST.VISUAL.BULLET + " " if all else "") + "Показания в помещение КТ"))
+        if not all:
+            if CheckableSections.BACKUPS in checkable_section_list:
+                robocopy_job_status_list: Result[list[RobocopyJobStatus]] = A.R_B.robocopy_job_status_list()
+                def job_status_item_label_function(job_status: RobocopyJobStatus, index: int) -> str:
+                    name: str = job_status.name
+                    source: str = job_status.source
+                    destination: str = job_status.destination 
+                    status: int | None = None
+                    date: str | None = None
+                    if job_status.active:
+                        date = "выполняется"
+                    else:
+                        if job_status.last_created is not None:
+                            date = f"{A.D_F.datetime(job_status.last_created)}"
+                        status = job_status.last_status
+                    return f" {CONST.VISUAL.BULLET} {self.bold(f'{name}:{source}{CONST.VISUAL.ARROW}{destination}')}" + ("" if status is None else f" [ {self.bold(str(status))} ]") + ("" if A.D_C.empty(date) else f"\n   {date}")
+                self.output.write_result(
+                    robocopy_job_status_list, False, label_function=job_status_item_label_function, separated_result_item=False, title=f" {CONST.VISUAL.BULLET} {self.bold('Название работы')}" + f" [ {self.bold('Статус')} ]" + f"\n   Дата создания\n{ConsoleAppsApi.LINE}")
+                
 
+
+    def polibase_restart(self, forced: bool = False) -> None:
+        if self.input.yes_no("Перезапустить"):
+            check_word: str = CONST.POLIBASE.NAME
+            test: bool = not (check_word == self.input.input(
+                f"Введите контрольное слово: {self.bold(check_word)}"))
+            if not test and A.C_R.polibase_accessibility(True) and not forced:
+                self.output.error(
+                    "Перезапуск Polibase: перезапуск невозможен - сервер доступен")
+            else:
+                notify: bool = test or self.input.yes_no("Уведомить пользователей", True)
+                title: str = f"Перезапуск Polibase{' test' if test else ''}"
+                polibase_host: str = HOSTS.POLIBASE_TEST.NAME if test else HOSTS.POLIBASE.NAME
+                self.output.write_line(A.L.it(
+                    f"{title}: Начат процесс закрытия программы Polibase на компьютерах."))
+                A.A_P.program_close_for_all(notify, None, test)
+                self.output.new_line()
+                self.output.write_line(A.L.it(
+                    f"{title}: Начат процесс перезагрузки сервера Polibase."))
+                A.A_P.restart(test)
+                while_not_do(lambda: not A.C_R.accessibility_by_ping(
+                    polibase_host), sleep_time=5)
+                self.output.new_line()
+                self.output.write_line(A.L.it(
+                     f"{title}: Начат процесс загрузки сервера Polibase."))
+                while_not_do(lambda: A.C_R.accessibility_by_ping(polibase_host), sleep_time=5)
+                self.output.new_line()
+                A.EV.wait_server_start(polibase_host)
+                self.output.write_line(A.L.it(f"{title}: Завершен процесс загрузки сервера Polibase."))
+                A.ME_P.notify_about_polibase_restarted(test)
+
+    def polibase_client_program_close(self, search_value: str | None = None) -> None:
+        for_all: bool = self.input.yes_no("Закрыть для всех пользователей", False, no_label=self.bold("Введите запрос для поиска компьютера"))
+        if for_all:
+            check_word: str = CONST.POLIBASE.NAME
+            test: bool = not (check_word == self.input.input(
+            f"Введите контрольное слово: {self.bold(check_word)}"))
+            A.A_P.program_close_for_all(True, self.input.input("Введите сообщение для пользователей Polibase"), test) 
+        else:
+            search_value = self.input.answer
+            workstation_list: list[Workstation] | None = None
+            try:
+                workstation_list = A.R_WS.by_any(search_value or self.input.input("Введите запрос для поиска компьютера"))
+                def every_action(workstation: Workstation) -> None:
+                    if A.A_P.client_program_close_for_workstation(workstation):
+                        self.output.good(f"Программа Polibase закрыта на компьютере {workstation.name}")
+                ResultTool.every(workstation_list, every_action)
+            except NotFound as error:
+                self.output.error(error.get_details())
+       
     @property
     def output(self) -> Output:
         return self.pih.output
 
     @property
     def input(self) -> Input:
         return self.pih.input
 
     def send_whatsapp_message(self, telephone_number: str, message: str) -> bool:
         return A.ME_WH_W.send(telephone_number, message, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.IT)
 
-    def find_mark(self, value: str = None) -> None:
+    def mark_find(self, value: str = None) -> None:
         self.output.mark.by_any(value or self.input.mark.any())
 
     def arg(self, index: int = 0, default_value: Any = None) -> Any:
         return self.session.arg(index, default_value)
 
     def register_ct_indications(self) -> None:
         text: str = f"число, которое может содержать дробную часть разделенную {self.bold('точкой')} или {self.bold('запятой')}"
@@ -96,15 +196,15 @@
         humidity: float = float_check_function(self.arg(1), False) or self.input.input(
             f"Введите значение {self.bold('влажности')} {number_format_notification_text}", check_function=float_check_function)
         indication: CTIndicationValue = CTIndicationValue(temperature, humidity)
         if A.A_I_CT.register(indication):
             with self.output.send_to_group(CONST.MESSAGE.WHATSAPP.GROUP.RD_INDICATIONS):
                 self.output.write_result(
                     Result(FIELD_COLLECTION.INDICATIONS.CT, indication), title=f"{self.get_formatted_given_name()}, отправил следующие показания в помещение КТ:")
-            self.output.good("спасибо, показания отправлены")
+            self.output.good("Спасибо, показания отправлены")
 
     def find_free_mark(self, value: str = None) -> None:
         self.output.mark.result(A.R_M.by_any(
             value or self.input.mark.any()), "Список свободных карт доступа:")
 
     def find_user(self, value: str = None) -> None:
         try:
@@ -122,16 +222,16 @@
         while True:
             password = self.input.user.generate_password(
                 True, password_settings)
             self.output.value("Пароль", password)
             if self.input.yes_no("Использовать", True):
                 break
         if self.input.yes_no("Отправить в ИТ отдел"):
-            A.L.from_it_bot(f"Сгенерированный пароль:")
-            A.L.from_it_bot(password)
+            A.L.it(f"Сгенерированный пароль:")
+            A.L.it(password)
         return password
 
     def make_mark_as_free(self, value: str = None) -> None:
         mark: Mark = self.input.mark.by_any(value)
         mark_type: int = EnumTool.get(MarkType, mark.type)
         if mark_type == MarkType.FREE:
             self.output.error(
@@ -206,34 +306,34 @@
 
     def bold(self, value: str) -> str:
         return self.output.bold(value)
 
     def italic(self, value: str) -> str:
         return self.output.italic(value)
 
-    def run_command(self, command_list: List[str] = None) -> None:
+    def run_command(self, command_list: list[str] = None) -> None:
         default_host: str = CONST.HOST.DC2.NAME
         host: str = None
         def get_command_list() -> list[str]:
             command_list: tuple[list[str], list[str]] = StringTool.dequotes(
                 self.pih.input.input("Введите команду"))
-            return list(filter(lambda item: not DataTool.is_empty(item), command_list[0] + command_list[1]))
+            return list(filter(lambda item: not A.D_C.empty(item), command_list[0] + command_list[1]))
         command_list = command_list or get_command_list()
-        use_psexec: bool = DataTool.is_empty([value for value in list(map(
+        use_psexec: bool = A.D_C.empty([value for value in list(map(
             lambda item: item.lower(), command_list)) if value in CONST.PSTOOLS.COMMAND_LIST])
         result: CompletedProcess = None
         if use_psexec:
-            if DataTool.is_empty(host):
+            if A.D_C.empty(host):
                 if self.input.yes_no(f"Использовать хост {self.bold(default_host)}, для выполнения команды", no_label=f"{self.bold('Или введите название хоста')}"):
                     host = default_host
                 else:
                     host = self.input.answer
             while True:
                 host = host.lower()
-                if A.C_RM.accessibility_by_ping(host, count=1):
+                if A.C_R.accessibility_by_ping(host, count=1):
                     self.output.write_line(
                         f"Команда будет запущена на хосте {self.bold(host)}\n")
                     break
                 else:
                     self.output.error(f"Хост {self.bold(host)} не доступен")
                     host = self.input.input(
                         "Введите имя хоста, на котором будет выполнена команда")
@@ -243,15 +343,15 @@
                 command_list, host, interactive=True, run_from_system_account=True, run_with_elevetion=True), True, True)
         else:
             self.output.write_line(
                 f"{self.get_formatted_given_name()}, ожидайте окончания выполнения команды...")
             result = A.PS.execute_command_list(
                 A.PS.create_command_list_for_pstools_command(command_list[0], command_list[1:]), True, True)
         result_out: str = result.stdout
-        if not DataTool.is_empty(result_out):
+        if not A.D_C.empty(result_out):
             self.output.write_line(result_out)
         if result.returncode != 0:
             error: str = result.stderr
             self.output.write_line(error)
 
     def create_new_mark(self):
 
@@ -320,15 +420,15 @@
     def user(self) -> User:
         return self.session.user
 
     @property
     def user_description(self) -> str:
         return A.D_F.description(self.user.description)
 
-    def send_workstation_message(self, recipient_name: str = None, use_dialog: bool = False) -> None:
+    def send_workstation_message(self, recipient_name: str = None, message: str | None = None, ask_for_use_dialog: bool = True) -> None:
         recipient: User | WorkstationDescription = None
         while True:
             try:
                 recipient = DataTool.get_first_item(
                     self.input.user.by_any(recipient_name, True))
                 if recipient is not None:
                     break
@@ -342,36 +442,41 @@
                     recipient_name = None
                     self.output.error(error.get_details())
         if isinstance(recipient, User) and ResultTool.is_empty(A.R_WS.by_login(recipient.samAccountName)):
             self.output.error(
                 f"Пользователь {recipient.name} ({recipient.samAccountName}) не залогинен ни за одним компьютером.")
         else:
             try:
-                use_dialog = use_dialog or self.input.yes_no("Начать диалог")
+                use_dialog: bool = False
+                if ask_for_use_dialog:
+                    use_dialog = A.D_C.empty(message) and self.input.yes_no("Начать диалог")
+                else:
+                    use_dialog = True
                 while True:
                     user_given_name: str = self.get_formatted_given_name(self.user_given_name)
                     if isinstance(recipient, User):
-                        message: str = self.input.message(
+                        message = message or self.input.message(
                             f"{user_given_name}, введите сообщение для пользователя {self.get_formatted_given_name(FullNameTool.to_given_name(recipient))}", f"Сообщение от {self.user_given_name} ({self.user_description}): {FullNameTool.to_given_name(recipient)}, ")
                         if A.ME_WS.to_user(recipient, message):
-                            self.output.good("сообщение отправлено")
+                            self.output.good("Сообщение отправлено")
                     else:
-                        message: str = self.input.message(
+                        message =  message or self.input.message(
                             f"{user_given_name}, введите сообщение для компьютера {recipient.name}", f"Сообщение от {self.user_given_name} ({self.user_description}): ")
                         if A.ME_WS.to_workstation(recipient, message):
-                            self.output.good("сообщение отправлено")
+                            self.output.good("Сообщение отправлено")
+                            message = None
                     if use_dialog:
                         self.output.separated_line()
                     else:
                         break
             except KeyboardInterrupt:
                 if use_dialog:
-                    A.O.error("Выход из диалога...")
+                    self.output.error("Выход из диалога...")
                 else:
-                    A.O.error("Отмена...")
+                    self.output.error("Отмена...")
 
     @property
     def user_given_name(self) -> str:
         return self.session.user_given_name
     
     def get_formatted_given_name(self, value: str = None) -> str:
         return self.output.user.get_formatted_given_name(value or self.user_given_name)
@@ -415,17 +520,17 @@
                 self.output.error("Ошибка")
         except KeyboardInterrupt:
             self.output.new_line()
             self.output.error("Отмена")
             self.output.new_line()
 
     def start_user_telephone_number_editor(self) -> None:
-        only_empty_phones_edit: bool = self.input.yes_no(
+        only_empty_telephone_number_edit: bool = self.input.yes_no(
             "Редактировать только телефоны, которые не заданы", True)
-        result: Result[list[User]] = A.R_U.list(True)
+        result: Result[list[User]] = A.R_U.all(True)
         for user in result.data:
             user: User = user
             if A.C_U.user(user):
                 if user.telephoneNumber is None:
                     self.output.error(f"{user.name}: нет телефона")
                     self.telephone_number_fix_action(user)
                 elif not A.C.telephone_number(user.telephoneNumber):
@@ -435,15 +540,15 @@
                         self.output.good(f"{user.name} телефон исправлен")
                         A.A_U.set_telephone_number(
                             user, fixed_telephone)
                     else:
                         self.output.yellow(
                             f"{user.name}: неправильный формат телефона ({user.telephoneNumber})")
                 else:
-                    if not only_empty_phones_edit:
+                    if not only_empty_telephone_number_edit:
                         self.output.good(
                             f"{user.name}: телефон присутствует")
                         self.telephone_number_fix_action(user)
             else:
                 self.output.notify(
                     f"{user.name}, похоже не пользователь, у которого должен быть номер телефона")
 
@@ -456,29 +561,29 @@
             if choose_user:
                 user_list = self.input.user.by_any(search_value, active)
             else:
                 result: Result[list[User]] = A.R_U.by_any(
                     self.input.user.title_any(), active)
                 user_list = result.data
             if property_name == USER_PROPERTY.USER_STATUS:
-                for status in [CONST.AD.ACTIVE_USERS_CONTAINER_DN, CONST.AD.INACTIVE_USERS_CONTAINER_DN]:
+                for status in [AD.ACTIVE_USERS_CONTAINER_DN, AD.INACTIVE_USERS_CONTAINER_DN]:
                     work_user_list: list[User] = self.pih.DATA.FILTER.users_by_dn(
-                        user_list, CONST.AD.INACTIVE_USERS_CONTAINER_DN if status == CONST.AD.ACTIVE_USERS_CONTAINER_DN else CONST.AD.ACTIVE_USERS_CONTAINER_DN)
+                        user_list, AD.INACTIVE_USERS_CONTAINER_DN if status == AD.ACTIVE_USERS_CONTAINER_DN else AD.ACTIVE_USERS_CONTAINER_DN)
                     for index, user in enumerate(work_user_list):
                         try:
                             self.output.user.result(Result(fields, [user]))
-                            if self.input.yes_no(f"{'Активировать' if status == CONST.AD.ACTIVE_USERS_CONTAINER_DN else 'Деактивировать' } пользователя"):
-                                if status == CONST.AD.ACTIVE_USERS_CONTAINER_DN:
+                            if self.input.yes_no(f"{'Активировать' if status == AD.ACTIVE_USERS_CONTAINER_DN else 'Деактивировать' } пользователя"):
+                                if status == AD.ACTIVE_USERS_CONTAINER_DN:
                                     if self.input.yes_no("Использовать шаблон для пользователя", True):
                                         user_container = self.input.user.template()
                                     else:
                                         user_container = self.input.user.container()
                                 else:
                                     user_container = UserContainer(
-                                        distinguishedName=CONST.AD.INACTIVE_USERS_CONTAINER_DN)
+                                        distinguishedName=AD.INACTIVE_USERS_CONTAINER_DN)
                                 if self.pih.ACTION.USER.set_status(user, status, user_container):
                                     self.output.good("Успешно")
                                 else:
                                     self.output.error("Ошибка")
                             else:
                                 self.output.new_line()
                                 self.output.error("Отмена")
```

### Comparing `pih-1.421/pih/const.py` & `pih-1.43/pih/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 ﻿from enum import *
 import os
-from typing import List
 
-from pih.collection import FieldItem, FieldItemList, LogCommandDescription, ParamItem, PasswordSettings, ServiceRoleDescription, SettingsValue, ResourceDescription, SiteResourceDescription, RobocopyJobDescription
+from pih.collection import FieldItem, FieldItemList, LogCommandDescription, ParamItem, PasswordSettings, ServiceRoleDescription, SettingsValue, ResourceDescription, SiteResourceDescription, PolibaseDocumentDescription, MedicalDirectionDescription
 
-#deprecated
-class DATA_EXTRACTOR:
+class DATA:
 
-    USER_NAME_FULL: str = "user_name_full"
-    USER_NAME: str = "user_name"
-    AS_IS: str = "as_is"
+    #deprecated
+    class EXTRACTOR:
+
+        USER_NAME_FULL: str = "user_name_full"
+        USER_NAME: str = "user_name"
+        AS_IS: str = "as_is"
+
+    class FORMATTER:
+
+        MY_DATETIME: str = "my_datetime"
 
 
 class USER_PROPERTY:
 
     TELEPHONE_NUMBER: str = "telephoneNumber"
     EMAIL: str = "mail"
     DN: str = "distinguishedName"
@@ -22,25 +27,126 @@
     DESCRIPTION: str = "description"
     PASSWORD: str = "password"
     USER_STATUS: str = "userStatus"
     NAME: str = "name"
 
 class BARCODE:
 
-    FORMAT_DEFAULT: str = "code128"
+    CODE128: str = "code128"
+    I25: str = "i25"
+
+class AD:
+
+    SEARCH_ATTRIBUTES: list[str] = [
+        USER_PROPERTY.LOGIN, USER_PROPERTY.NAME]
+    SEARCH_ATTRIBUTE_DEFAULT: str = SEARCH_ATTRIBUTES[0]
+    DOMAIN_NAME: str = "fmv"
+    DOMAIN_ALIAS: str = "pih"
+    DOMAIN_SUFFIX: str = "lan"
+    DOMAIN: str = f"{DOMAIN_NAME}.{DOMAIN_SUFFIX}"
+    DOMAIN_MAIN: str = DOMAIN
+    USER_HOME_FOLDER_DISK: str = "U:"
+    OU: str = "OU="
+    ROOT_CONTAINER_DN: str = f"{OU}Unit,DC={DOMAIN_NAME},DC={DOMAIN_SUFFIX}"
+    WORKSTATIONS_CONTAINER_DN: str = f"{OU}Workstations,{ROOT_CONTAINER_DN}"
+    USERS_CONTAINER_DN_SUFFIX: str = f"Users,{ROOT_CONTAINER_DN}"
+    ACTIVE_USERS_CONTAINER_DN: str = f"{OU}{USERS_CONTAINER_DN_SUFFIX}"
+    INACTIVE_USERS_CONTAINER_DN: str = f"{OU}dead{USERS_CONTAINER_DN_SUFFIX}"
+    PATH_ROOT: str = f"\\\{DOMAIN_MAIN}"
+    SEARCH_ALL_PATTERN: str = "*"
+    GROUP_CONTAINER_DN: str = f"{OU}Groups,{ROOT_CONTAINER_DN}"
+    JOB_POSITION_CONTAINER_DN: str = f"{OU}Job positions,{GROUP_CONTAINER_DN}"
+    LOCATION_JOINER: str = ":"
+    TEMPLATED_USER_SERACH_TEMPLATE: str = "_*_"
+    PROPERTY_ROOT_DN: str = f"{OU}Property,{GROUP_CONTAINER_DN}"
+    PROPERTY_WS_DN: str = f"{OU}WS,{PROPERTY_ROOT_DN}"
+
+    USER_ACCOUNT_CONTROL: list[str] = [
+        "SCRIPT",
+        "ACCOUNTDISABLE",
+        "RESERVED",
+        "HOMEDIR_REQUIRED",
+        "LOCKOUT",
+        "PASSWD_NOTREQD",
+        "PASSWD_CANT_CHANGE",
+        "ENCRYPTED_TEXT_PWD_ALLOWED",
+        "TEMP_DUPLICATE_ACCOUNT",
+        "NORMAL_ACCOUNT",
+        "RESERVED",
+        "INTERDOMAIN_TRUST_ACCOUNT",
+        "WORKSTATION_TRUST_ACCOUNT",
+        "SERVER_TRUST_ACCOUNT",
+        "RESERVED",
+        "RESERVED",
+        "DONT_EXPIRE_PASSWORD",
+        "MNS_LOGON_ACCOUNT",
+        "SMARTCARD_REQUIRED",
+        "TRUSTED_FOR_DELEGATION",
+        "NOT_DELEGATED",
+        "USE_DES_KEY_ONLY",
+        "DONT_REQ_PREAUTH",
+        "PASSWORD_EXPIRED",
+        "TRUSTED_TO_AUTH_FOR_DELEGATION",
+        "RESERVED",
+        "PARTIAL_SECRETS_ACCOUNT"
+    ]
+
+    WORKSTATION_PREFIX_LIST: list[str] = [
+        "ws-", "nb-", "fmvulianna"]
+
+    ADMINISTRATOR: str = "Administrator"
+    ADMINISTRATOR_PASSOWORD: str = "Fortun@90"
+
+    CALL_CENTRE_ADMINISTRATOR: str = "callCentreAdmin"
+
+    MARKETER: str = "marketer"
+
+    class JobPisitions(Enum):
+        HR: int = auto()
+        IT: int = auto()
+        CALL_CENTRE: int = auto()
+        REGISTRATOR: int = auto()
+        RD: int = auto()
+
+    class Groups(Enum):
+        TimeTrackingReport: int = auto()
+        Inventory: int = auto()
+        Polibase: int = auto()
+        Admin: int = auto()
+        ServiceAdmin: int = auto()
+        CardRegistry: int = auto()
+        PolibaseUsers: int = auto()
+        RD: int = auto()
+        IndicationWatcher: int = auto()
+
+    class WSProperies(Enum):
+
+        Watchable: int = 1
+        Shutdownable: int = 2
+        Rebootable: int = 4
+
+class FONT:
+
+    FOR_PDF: str = "DejaVuSerif"
 
 class FILE:
 
     class EXTENSION:
 
         EXCEL_OLD: str = "xls"
         EXCEL_NEW: str = "xlsx"
         JPEG: str = "jpeg"
+        JPG: str = "jpg"
         PNG: str = "png"
+        PDF: str = "pdf"
+        TXT: str = "txt"
         PYTHON: str = "py"
+        BASE64: str = "base64"
+        EXE: str = "exe"
+        TRUE_TYPE_FONT: str = "ttf"
 
 class HOSTS:
 
     class BACKUP_WORKER:
     
         NAME: str = "backup_worker"
         ALIAS: str = "backup_worker"
@@ -52,14 +158,25 @@
         IP: str = "192.168.254.102"
 
     class WS255:
     
         NAME: str = "ws-255"
         IP: str = "192.168.100.138"
 
+    class WS816:
+        
+        NAME: str = "ws-816"
+        IP: str = "192.168.254.81"
+
+    class WS735:
+        
+        NAME: str = "ws-735"
+        IP: str = "192.168.254.102"
+        ALIAS: str = "shared_disk_owner"
+
     class DC1:
     
         NAME: str = "fmvdc1.fmv.lan"
         ALIAS: str = "dc1"
         IP: str = "192.168.100.4"
 
     class DC2:
@@ -77,15 +194,15 @@
         #shit - cause polibase is not accessable
         NAME: str = "fmvpolibase1.fmv.lan"
         ALIAS: str = "polibase"
         IP: str = "192.168.100.3"
 
     class POLIBASE_TEST:
 
-        NAME: str = "polibase_test"
+        NAME: str = "fmvpolibase2.fmv.lan"
         ALIAS: str = "polibase_test"
         IP: str = "192.168.110.140"
 
     class _1C:
 
         NAME: str = "1c"
         ALIAS: str = "1c"
@@ -99,47 +216,55 @@
 
     class PACS_ARCHVE:
 
         NAME: str = "pacs_archive"
         ALIAS: str = "ea_archive"
         IP: str = "192.168.110.108"
 
+class URLS:
+
+    PYPI: str = "https://pypi.python.org/pypi/pih/json"
+
 
 class CONST:
 
     class TEST:
 
         WS: str = HOSTS.DEVELOPER.NAME
 
     GROUP_PREFIX: str = "group:"
 
-    SITE_ADDRESS: str = "pacifichosp.com"
-    MAIL_PREFIX: str = "mail"
     SITE_PROTOCOL: str = "https://"
-    UNTRUST_SITE_PROTOCOL: str = "http://"
-    EMAIL_ADDRESS: str = f"{MAIL_PREFIX}.{SITE_ADDRESS}"
+    UNTRUST_SITE_PROTOCOL: str = "http://" 
+    
+    SITE_ADDRESS: str = "pacifichosp.com"
+    MAIL_ADDRESS: str = f"mail.{SITE_ADDRESS}"
     WIKI_ADDRESS: str = f"{UNTRUST_SITE_PROTOCOL}wiki"
+
     INTERNATIONAL_TELEPHONE_NUMBER_PREFIX: str = "7"
     TELEPHONE_NUMBER_PREFIX: str = "+" + INTERNATIONAL_TELEPHONE_NUMBER_PREFIX
     INTERNAL_TELEPHONE_NUMBER_PREFIX: str = "тел."
 
     DATE_TIME_SPLITTER: str = "T"
     TIME_FORMAT: str = "%H:%M:00"
     SECONDLESS_TIME_FORMAT: str = "%H:%M"
     DATE_TIME_FORMAT: str = f"%Y-%m-%d{DATE_TIME_SPLITTER}{TIME_FORMAT}"
     DATE_FORMAT: str = "%d.%m.%Y"
 
+    YEARLESS_DATE_FORMAT: str = "%d.%m"
+
+    MY_DATE_FORMAT: str = "%d.%m.%Y %H:%M:%S"
+
     API_SITE_ADDRESS: str = f"api.{SITE_ADDRESS}"
 
     BITRIX_SITE_URL: str = "bitrix.cmrt.ru"
 
-    PYPI_URL: str = "https://pypi.python.org/pypi/pih/json"
-
     class DATA_STORAGE:
 
+        DADATA_TOKEN: str = "147c0cd53d67fb4e48e379336c5794ae146c9621"
         DATE_TIME_SPLITTER: str = " "
         DATE_FORMAT: str = "%Y-%m-%d"
         TIME_FORMAT: str = "%H:%M:00"
         DATE_TIME_FORMAT: str = f"{DATE_FORMAT}{DATE_TIME_SPLITTER}{TIME_FORMAT}"
 
     class CACHE:
         
@@ -158,21 +283,24 @@
         REPORT_DAY_PERIOD_DEFAULT: int = 15
 
     class MESSAGE:
 
         class WHATSAPP:
 
             SITE_NAME: str = "https://wa.me/"
-            SEND_TO_TEMPLATE: str = SITE_NAME + "{}?text={}"
+            SEND_MESSAGE_TO_TEMPLATE: str = SITE_NAME + "{}?text={}"
 
+            GROUP_SUFFIX: str = "@g.us"
 
             class GROUP(Enum):
 
                 RD: str = "79146947050-1595848245@g.us"
-                RD_INDICATIONS: str = "120363084280723039@g.us"
+                CT_INDICATIONS: str = "120363084280723039@g.us"
+                DOCUMENTS_WORK_STACK: str = '120363115241877592@g.us'
+                DOCUMENTS_WORK_STACK_TEST: str = '120363128816931482@g.us'
 
             class WAPPI:
 
                 PROFILE_SUFFIX: str = "profile_id="
                 URL_API: str = "https://wappi.pro/api"
                 URL_API_SYNC: str = f"{URL_API}/sync"
                 URL_MESSAGE: str = f"{URL_API_SYNC}/message"
@@ -188,15 +316,15 @@
 
                 class PROFILE(Enum):
                     IT: str = "e6706eaf-ae17"
                     CALL_CENTRE: str = "56ad2cb1-a5ac"
                     MARKETER: str = "c31db01c-b6d6"
                     DEFAULT: str = CALL_CENTRE
                     
-                AUTHORICATION: str = "6b356d3f53124af3078707163fdaebca3580dc38"
+                AUTHORIZATION: str = "6b356d3f53124af3078707163fdaebca3580dc38"
             
     class PYTHON:
 
         EXECUTOR: str = "py"
         PYPI: str = "pip"
 
     class SERVICE:
@@ -204,30 +332,35 @@
         NAME: str = "service"
 
     class FACADE:
 
         SERVICE_FOLDER_SUFFIX: str = "Core"
         PATH: str = "\\\\pih\\facade\\"
 
+    class VALENTA:
+
+        PROCESS_NAME: str = "Vlwin"
+
     class PSTOOLS:
 
         NAME: str = "pstools"
         PS_EXECUTOR: str = "psexec"
         PS_KILL_EXECUTOR: str = "pskill"
+        PS_PING: str = "psping"
 
-        COMMAND_LIST: List[str] = [
+        COMMAND_LIST: list[str] = [
             PS_KILL_EXECUTOR,
             "psfile",
             "psgetsid",
             "psinfo",
             "pslist",
             "psloggedon",
             "psloglist",
             "pspasswd",
-            "psping",
+            PS_PING,
             "psservice",
             "psshutdown",
             "pssuspend"
         ]
 
         NO_BANNER: str = "-nobanner"
         ACCEPTEULA: str = "-accepteula"
@@ -259,104 +392,15 @@
         USER_DATA_INPUT_TIMEOUT: int = 180
 
         class InteraptionTypes:
 
             INTERNAL: int = 1
             TIMEOUT: int = 2
 
-    class AD:
-
-        SEARCH_ATTRIBUTES: List[str] = [
-            USER_PROPERTY.LOGIN, USER_PROPERTY.NAME]
-        SEARCH_ATTRIBUTE_DEFAULT: str = SEARCH_ATTRIBUTES[0]
-        DOMAIN_NAME: str = "fmv"
-        DOMAIN_ALIAS: str = "pih"
-        DOMAIN_SUFFIX: str = "lan"
-        DOMAIN: str = f"{DOMAIN_NAME}.{DOMAIN_SUFFIX}"
-        DOMAIN_MAIN: str = DOMAIN
-        USER_HOME_FOLDER_DISK: str = "U:"
-        OU: str = "OU="
-        ROOT_CONTAINER_DN: str = f"{OU}Unit,DC={DOMAIN_NAME},DC={DOMAIN_SUFFIX}"
-        WORKSTATIONS_CONTAINER_DN: str = f"{OU}Workstations,{ROOT_CONTAINER_DN}"
-        USERS_CONTAINER_DN_SUFFIX: str = f"Users,{ROOT_CONTAINER_DN}"
-        ACTIVE_USERS_CONTAINER_DN: str = f"{OU}{USERS_CONTAINER_DN_SUFFIX}"
-        INACTIVE_USERS_CONTAINER_DN: str = f"{OU}dead{USERS_CONTAINER_DN_SUFFIX}"
-        PATH_ROOT: str = f"\\\{DOMAIN_MAIN}"
-        SEARCH_ALL_PATTERN: str = "*"
-        GROUP_CONTAINER_DN: str = f"{OU}Groups,{ROOT_CONTAINER_DN}"
-        JOB_POSITION_CONTAINER_DN: str = f"{OU}Job positions,{GROUP_CONTAINER_DN}"
-        LOCATION_JOINER: str = ":"
-        TEMPLATED_USER_SERACH_TEMPLATE: str = "_*_"
-        PROPERTY_ROOT_DN: str = f"{OU}Property,{GROUP_CONTAINER_DN}"
-        PROPERTY_WS_DN: str = f"{OU}WS,{PROPERTY_ROOT_DN}"
-
-        USER_ACCOUNT_CONTROL: List[str] = [
-            "SCRIPT",
-            "ACCOUNTDISABLE",
-            "RESERVED",
-            "HOMEDIR_REQUIRED",
-            "LOCKOUT",
-            "PASSWD_NOTREQD",
-            "PASSWD_CANT_CHANGE",
-            "ENCRYPTED_TEXT_PWD_ALLOWED",
-            "TEMP_DUPLICATE_ACCOUNT",
-            "NORMAL_ACCOUNT",
-            "RESERVED",
-            "INTERDOMAIN_TRUST_ACCOUNT",
-            "WORKSTATION_TRUST_ACCOUNT",
-            "SERVER_TRUST_ACCOUNT",
-            "RESERVED",
-            "RESERVED",
-            "DONT_EXPIRE_PASSWORD",
-            "MNS_LOGON_ACCOUNT",
-            "SMARTCARD_REQUIRED",
-            "TRUSTED_FOR_DELEGATION",
-            "NOT_DELEGATED",
-            "USE_DES_KEY_ONLY",
-            "DONT_REQ_PREAUTH",
-            "PASSWORD_EXPIRED",
-            "TRUSTED_TO_AUTH_FOR_DELEGATION",
-            "RESERVED",
-            "PARTIAL_SECRETS_ACCOUNT"
-        ]
-
-        WORKSTATION_PREFIX_LIST: List[str] = [
-            "ws-", "nb-", "fmvulianna"]
-
-        ADMINISTRATOR: str = "Administrator"
-        ADMINISTRATOR_PASSOWORD: str = "Fortun@90"
-
-        CALL_CENTRE_ADMINISTRATOR: str = "callCentreAdmin"
-
-        MARKETER: str = "marketer"
-
-        class JobPisitions(Enum):
-            HR: int = auto()
-            IT: int = auto()
-            CALL_CENTRE: int = auto()
-            REGISTRATOR: int = auto()
-            RD: int = auto()
-
-        class Groups(Enum):
-            TimeTrackingReport: int = auto()
-            Inventory: int = auto()
-            Polibase: int = auto()
-            Admin: int = auto()
-            ServiceAdmin: int = auto()
-            CardRegistry: int = auto()
-            PolibaseUsers: int = auto()
-            RD: int = auto()
-            IndicationWatcher: int = auto()
-
-        class WSProperies(Enum):
-    
-            Watchable: int = 1
-            Shutdownable: int = 2
-            Rebootable: int = 4
-
+   
     class NAME_POLICY:
 
         PARTS_LIST_MIN_LENGTH: int = 3
         PART_ITEM_MIN_LENGTH: int = 3
 
     class RPC:
 
@@ -371,31 +415,33 @@
         TIMEOUT: int = None
         TIMEOUT_FOR_PING: int = 2
 
     HOST = HOSTS()
 
     class POLIBASE:
 
+        NAME: str = "Polibase"
+
         PROCESS_NAME: str = "Polibase ODAC"
 
         PRERECORDING_PIN: int = 10
         RESERVED_TIME_A_PIN: int = 5
         RESERVED_TIME_B_PIN: int = 6
         RESERVED_TIME_C_PIN: int = 7
 
-        CARD_REGISTRY_FOLDER_NAME_CHECK_PATTERN: List[str] = [
+        CARD_REGISTRY_FOLDER_NAME_CHECK_PATTERN: list[str] = [
         "п", "т", "b", "p", "t", "б"]
     
         #145 - Средний Медицинский Персонал
         #300 - Реанимация
         #361 - Операционная блок
         #421 - СМП
         #221 -
         #229 -
-        CABINET_NO_EXCLUDE_FROM_VISIT_RESULT: List[int] = [145, 221, 229, 300, 361, 421]
+        CABINET_NO_EXCLUDE_FROM_VISIT_RESULT: list[int] = [145, 221, 229, 300, 361, 421]
         
         #147 - УЗИ
         #201 - ЭНДОСКОПИЯ
         #202 - МРТ
         #203 - КТ
 
         class APPOINTMENT_SERVICE_GROUP_ID(Enum):
@@ -407,15 +453,15 @@
         APPOINTMENT_SERVICE_GROUP_NAME: dict = {
             APPOINTMENT_SERVICE_GROUP_ID.ULTRASOUND: "ультразвуковое исследование",
             APPOINTMENT_SERVICE_GROUP_ID.ENDOSCOPY: "эндоспопичекое исследование",
             APPOINTMENT_SERVICE_GROUP_ID.MRI: "МРТ исследование", 
             APPOINTMENT_SERVICE_GROUP_ID.CT: "рентген исследование"
         }
 
-        STATUS_EXCLUDE_FROM_VISIT_RESULT: List[int] = [63]
+        STATUS_EXCLUDE_FROM_VISIT_RESULT: list[int] = [63]
 
         ###
 
         TELEGRAM_BOT_URL: str = "https://t.me/pacifichospital_bot"
 
         REVIEW_ACTION_URL: str = "https://forms.gle/qriwujnAknYXga4eA"
 
@@ -445,17 +491,17 @@
 
         PERSON_REVIEW_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION: str = PERSON_REVIEW_NOTIFICATION_TEXT_BASE + SEND_REVIEW_ACTION_URL_TEXT
 
         ASK_TO_SEND_REVIEW_ACTION_TEXT: str = ". Согласны ли Вы пройти опрос?"
 
         PERSON_REVIEW_NOTIFICATION_TEXT: str = PERSON_REVIEW_NOTIFICATION_TEXT_BASE + ASK_TO_SEND_REVIEW_ACTION_TEXT
 
-        YES_ANSWER: List[str] = ["да", "согласен", "согласна", "ok", "ок", "yes", "хорошо", "ага"]
+        YES_ANSWER: list[str] = ["да", "согласен", "согласна", "ok", "ок", "yes", "хорошо", "ага"]
 
-        NO_ANSWER: List[str] = ["нет", "не согласен", "не согласна", "no", "занят"]
+        NO_ANSWER: list[str] = ["нет", "не согласен", "не согласна", "no", "занят"]
 
         TAKE_TELEGRAM_BOT_URL_TEXT: str = "*{name}*, отправляем Вам ссылку:\n"
 
         PERSONLESS_TAKE_TELEGRAM_BOT_URL_TEXT: str = "Отправляем Вам ссылку:\n"
 
         TAKE_REVIEW_ACTION_URL_TEXT: str = "*{name}*, отправляем Вам ссылку для прохождения опроса:"
 
@@ -470,26 +516,41 @@
         class BARCODE:
             
             class PERSON:
                 IMAGE_FORMAT: str =  FILE.EXTENSION.JPEG
             class PERSON_CARD_FOLDER:
                 IMAGE_FORMAT: str = FILE.EXTENSION.PNG
             
-            FORMAT: str = BARCODE.FORMAT_DEFAULT
+            ACTUAL_FORMAT: str = BARCODE.CODE128
+            OLD_FORMAT: str = BARCODE.I25
+
+            SUPPORT_FORMATS: list[str] = [ACTUAL_FORMAT, OLD_FORMAT]
 
             NEW_PATTERN: str = "new_"
 
             @staticmethod
             def get_file_name(pin: int, with_extension: bool = False) -> str:
                 extension: str = f".{CONST.POLIBASE.BARCODE.PERSON.IMAGE_FORMAT}" if with_extension else ""
                 return f"{CONST.POLIBASE.BARCODE.NEW_PATTERN}{pin}{extension}"
+            
+        class DOCUMENT_DESCRIPTIONS(Enum):
+
+            HOLTER_JOURNAL: PolibaseDocumentDescription = PolibaseDocumentDescription("Дневник суточного мониторинга ЭКГ", 70, 70, 80)
+            PATIENT_CARD_AMBULATORY: PolibaseDocumentDescription = PolibaseDocumentDescription("Медицинская карта\nпациента, получившего медицинскую помощь\nв амбулаторных условиях", 70, 120, 120)
+            PROCESSING_PRESONAL_DATA_CONSENT: PolibaseDocumentDescription = PolibaseDocumentDescription("согласие\nпациента на обработку персональных данных", 70, 70, 120, 1)
+            INFORMED_VOLUNTARY_MEDICAL_INVENTION_CONSENT: PolibaseDocumentDescription = PolibaseDocumentDescription("информированное добровольное согласие\nна медицинское вмешательство", 70, 70, 120, 1)
+            INFORMED_VOLUNTARY_MEDICAL_INVENTION_CONSENT_SPECIFIC: PolibaseDocumentDescription = PolibaseDocumentDescription("информированное добровольное согласие на виды медицинских\nвмешательств, включенные в перечень определенных видов\nмедицинских вмешательств, на которые граждане дают\nинформированное добровольное согласие при выборе врача и\nмедицинской организации для получения первичной медико-\nсанитарной помощи", 70, 70, 280, 2)
+
+            @staticmethod
+            def sorted() -> list:
+                return sorted(CONST.POLIBASE.DOCUMENT_DESCRIPTIONS, key=lambda item: item.value.title_height, reverse=True)
     
     class VISUAL:
 
-        NUMBER_SYMBOLS: List[str] = [
+        NUMBER_SYMBOLS: list[str] = [
            "0️⃣",
            "1️⃣",
            "2️⃣",
            "3️⃣", 
            "4️⃣",
            "5️⃣",
            "6️⃣",
@@ -499,55 +560,87 @@
            "🔟"
         ]
 
         ARROW: str = "➜"
 
         BULLET: str = "•" 
 
-class RESOURCE_DESCRIPTION_COLLECTION:
+class RESOURCE:
+
+    class DESCRIPTIONS:
     
-    INTERNET: ResourceDescription = ResourceDescription(
-        "77.88.55.242", "Интернет соединение")
+        INTERNET: ResourceDescription = ResourceDescription(
+            "77.88.55.242", "Интернет соединение")
+        
+        VPN_PACS_SPB: ResourceDescription = ResourceDescription(
+            "192.168.5.3", "VPN соединение для PACS SPB", (2, 100, 5))
+        PACS_SPB: ResourceDescription = ResourceDescription(
+            "10.76.12.124:4242", "Соединение PACS SPB", (2, 100, 5))
+
+        POLIBASE: ResourceDescription = ResourceDescription("polibase", "Polibase", inaccessibility_check_values=(2, 10000, 15))
+
+        SITE_LIST: list[SiteResourceDescription] = [
+            SiteResourceDescription(
+                        CONST.SITE_ADDRESS, f"Сайт компании: {CONST.SITE_ADDRESS}", check_certificate_status=True, check_free_space_status=False),
+            SiteResourceDescription(CONST.MAIL_ADDRESS,
+                        f"Сайт корпоративной почты: {CONST.MAIL_ADDRESS}", check_certificate_status=True, check_free_space_status=True, driver_name="/dev/mapper/centos_tenant26--02-var"),
+            SiteResourceDescription(CONST.API_SITE_ADDRESS,
+                                    f"Api сайта {CONST.SITE_ADDRESS}: {CONST.API_SITE_ADDRESS}", check_certificate_status=True, check_free_space_status=False),
+            SiteResourceDescription(CONST.BITRIX_SITE_URL, f"Сайт Битрикс ЦМРТ24: {CONST.BITRIX_SITE_URL}")
+        ]
     
-    VPN_PACS: ResourceDescription = ResourceDescription("192.168.5.3", "VPN соединение для PACS SPB")
-    PACS: ResourceDescription = ResourceDescription(
-        "10.76.12.124:4242", "Соединение PACS SPB", (3, 100, 5))
-
-    POLIBASE: ResourceDescription = ResourceDescription("polibase", "Polibase", inaccessibility_check_values=(2, 10000, 15))
-
-    SITE_LIST: List[SiteResourceDescription] = [
-        SiteResourceDescription(
-                    CONST.SITE_ADDRESS, f"Сайт компании: {CONST.SITE_ADDRESS}", check_certificate_status=True, check_free_space_status=False),
-        SiteResourceDescription(CONST.EMAIL_ADDRESS,
-                    f"Сайт корпоративной почты: {CONST.EMAIL_ADDRESS}", check_certificate_status=True, check_free_space_status=True, driver_name="/dev/mapper/centos_tenant26--02-var"),
-        SiteResourceDescription(CONST.API_SITE_ADDRESS,
-                                f"Api сайта {CONST.SITE_ADDRESS}: {CONST.API_SITE_ADDRESS}", check_certificate_status=True, check_free_space_status=False),
-        SiteResourceDescription(CONST.BITRIX_SITE_URL, f"Сайт Битрикс ЦМРТ24: {CONST.BITRIX_SITE_URL}")
-    ]
+    class INACCESSABLE_REASON(Enum):
+
+        SERTIFICATE_ERROR: str = "Ошибка проверки сертификата"
+
+class MEDICAl_DOCUMENT:
+
+    class DIRECTION_TYPES(Enum):
+            
+        MRI: MedicalDirectionDescription = MedicalDirectionDescription(("Магнитно-резонансная томография", ), "МРТ")
+        CT: MedicalDirectionDescription = MedicalDirectionDescription(("Компьютерная томография", ), "КТ")
+        ULTRASOUND: MedicalDirectionDescription = MedicalDirectionDescription(("ультразвуковая допплерография", ), "УЗИ")
 
 class CheckableSections(Enum):
 
     RESOURCES: int = auto()
     WS: int = auto()
     PRINTER: int = auto()
     INDICATIONS: int = auto()
+    BACKUPS: int = auto()
 
+    @staticmethod
     def all() :
         return [item for item in CheckableSections]
 
 class PATH_SHARE:
 
     NAME: str = "shares"
-    PATH: str = os.path.join(CONST.AD.PATH_ROOT, NAME)
+    PATH: str = os.path.join(AD.PATH_ROOT, NAME)
 
 class PATH_SCAN:
     
     NAME: str = "scan"
-    PATH: str = os.path.join(CONST.AD.PATH_ROOT, NAME)
+    VALUE: str = os.path.join(AD.PATH_ROOT, NAME)
+
+class PATH_SCAN_TEST:
+    
+    NAME: str = "test"
+    VALUE: str = os.path.join(PATH_SCAN.VALUE, NAME)
+
+
+class PATH_WS_816_SCAN:
+    
+    NAME: str = r"C$\Users\Nurse\Documents\Scanned Documents"
+    VALUE: str = os.path.join(r"\\", HOSTS.WS816.NAME, NAME)
 
+class PATH_OMS:
+    
+    NAME: str = "oms"
+    VALUE: str = os.path.join(AD.PATH_ROOT, NAME)
 
 class PATH_IT:
 
     NAME: str = "5. IT"
     NEW_EMPLOYEES_NAME: str = "New employees"
     ROOT: str = os.path.join(PATH_SHARE.PATH, NAME)
 
@@ -556,19 +649,49 @@
         return os.path.join(os.path.join(PATH_IT.ROOT, PATH_IT.NEW_EMPLOYEES_NAME), name)
 
 class PATH_APP:
 
     NAME: str = "apps"
     FOLDER: str = os.path.join(CONST.FACADE.PATH, NAME)
 
+class PATH_DOCS:
+    
+    NAME: str = f"Docs{CONST.FACADE.SERVICE_FOLDER_SUFFIX}"
+    FOLDER: str = os.path.join(CONST.FACADE.PATH, NAME)
+
+class PATH_FONTS:
+
+    NAME: str = "fonts"
+    FOLDER: str = os.path.join(PATH_DOCS.FOLDER, NAME)
+
+    @staticmethod
+    def get(name: str) -> str:
+        from pih.tools import PathTool
+        return os.path.join(PATH_FONTS.FOLDER, PathTool.add_extension(name, FILE.EXTENSION.TRUE_TYPE_FONT))
+
 class PATH_APP_DATA:
 
     NAME: str = "data"
     FOLDER: str = os.path.join(PATH_APP.FOLDER, NAME)
 
+    OCR_RESULT_NAME: str = "ocr result"
+    OCR_RESULT_FOLDER: str =  os.path.join(FOLDER, OCR_RESULT_NAME)
+
+class PATH_MOBILE_HELPER:
+
+    NAME: str = "mobile helper"
+    FOLDER: str = os.path.join(PATH_APP_DATA.FOLDER, NAME)
+
+    QR_CODE_NAME: str = "qr code"
+    QR_CODE_FOLDER: str =  os.path.join(FOLDER, QR_CODE_NAME)
+
+    INCOME_IMAGES_NAME: str = "income images"
+    INCOME_IMAGES_FOLDER: str =  os.path.join(FOLDER, INCOME_IMAGES_NAME)
+
+
 class PATH_POLIBASE_APP_DATA:
     
     NAME: str = "polibase"
     FOLDER: str = os.path.join(PATH_APP_DATA.FOLDER, NAME)
     PERSON_CARD_FOLDER: str = os.path.join(FOLDER, "person card folder")
 
     SERVICE_FOLDER_PATH: str = os.path.join(CONST.FACADE.PATH, f"{NAME}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}")
@@ -576,16 +699,20 @@
     class SETTINGS:
         MAIN: str = "polibase_main_settings.vbs"
         TEST: str = "polibase_test_settings.vbs"
 
 class PATH_USER:
 
     NAME: str = "homes"
-    HOME_FOLDER: str = os.path.join(CONST.AD.PATH_ROOT, NAME)
-    HOME_FOLDER_FULL: str = os.path.join(CONST.AD.PATH_ROOT, NAME)
+    HOME_FOLDER: str = os.path.join(AD.PATH_ROOT, NAME)
+    HOME_FOLDER_FULL: str = os.path.join(AD.PATH_ROOT, NAME)
+
+    @staticmethod
+    def private_folder(login: str) -> str:
+        return os.path.join(PATH_USER.HOME_FOLDER, login)
 
     @staticmethod
     def get_document_name(user_name: str, login: str = None) -> str:
         return PATH_IT.NEW_EMPLOYEE(user_name) + (f" ({login})" if login else "") + ".docx"
 
 class PATH_POLIBASE:
     
@@ -594,15 +721,15 @@
     PERSON_CARD_FOLDER: str = PATH_POLIBASE_APP_DATA.PERSON_CARD_FOLDER
 
     @staticmethod
     def get_person_folder(pin: int, test: bool = False) -> str:
         root: str = PATH_POLIBASE.NAME
         if test:
             if root.find(".") != -1:
-                root_parts: List = root.split(".")
+                root_parts: list = root.split(".")
                 root_parts[0] += PATH_POLIBASE.TEST_SUFFIX
                 root = ".".join(root_parts)
             else:
                 root += PATH_POLIBASE.TEST_SUFFIX
         return os.path.join(os.path.join(f"//{root}", "polibaseData", "PERSONS"), str(pin))
 
 class PATH_WS:
@@ -619,20 +746,27 @@
         ROOT: str = os.path.join(CONST.FACADE.PATH, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
     
 
 class PATHS:
 
     SHARE: PATH_SHARE = PATH_SHARE()
     SCAN: PATH_SCAN = PATH_SCAN()
+    SCAN_TEST = PATH_SCAN_TEST()
+    WS_816_SCAN: PATH_WS_816_SCAN = PATH_WS_816_SCAN()
+    OMS: PATH_OMS = PATH_OMS()
     IT: PATH_IT = PATH_IT()
     USER: PATH_USER = PATH_USER()
     POLIBASE: PATH_POLIBASE = PATH_POLIBASE()
     POLIBASE_APP_DATA: PATH_POLIBASE_APP_DATA = PATH_POLIBASE_APP_DATA()
     WS: PATH_WS = PATH_WS()
     BACKUP: PATH_BACKUP = PATH_BACKUP()
+    DOCS: PATH_DOCS = PATH_DOCS()
+    FONTS: PATH_FONTS = PATH_FONTS()
+    MOBILE_HELPER: PATH_MOBILE_HELPER = PATH_MOBILE_HELPER()
+    APP_DATA: PATH_APP_DATA = PATH_APP_DATA()
 
 class MarkType(Enum):
 
     NORMAL: int = auto()
     FREE: int = auto()
     GUEST: int = auto()
     TEMPORARY: int = auto()
@@ -918,15 +1052,15 @@
 
         CT: FieldItemList = FieldItemList(
             FieldItem(FIELD_NAME_COLLECTION.TEMPERATURE, "Температура", data_formatter="{data}°C"),
             FieldItem(FIELD_NAME_COLLECTION.HUMIDITY, "Влажность", data_formatter="{data}%")
         )
 
         CT_WITH_TIMESTAMP: FieldItemList = FieldItemList(CT,
-                                              FieldItem(FIELD_NAME_COLLECTION.TIMESTAMP, "Время измерения"))
+                                              FieldItem(FIELD_NAME_COLLECTION.TIMESTAMP, "Время измерения", data_formatter=f"{DATA.FORMATTER.MY_DATETIME}"))
 
 
 class FIELD_COLLECTION_ALIAS(Enum):
     TIME_TRACKING: FieldItem = FIELD_COLLECTION.ORION.TIME_TRACKING
     PERSON: FieldItem = FIELD_COLLECTION.ORION.PERSON
     TEMPORARY_MARK: FieldItem = FIELD_COLLECTION.ORION.TEMPORARY_MARK
     POLIBASE_PERSON: FieldItem = FIELD_COLLECTION.POLIBASE.PERSON
@@ -935,15 +1069,17 @@
     PERSON_EXTENDED: FieldItem = FIELD_COLLECTION.ORION.PERSON_EXTENDED
     WORKSTATION: FieldItem = FIELD_COLLECTION.AD.WORKSTATION
     USER_WORKSTATION: FieldItem = FIELD_COLLECTION.AD.USER_WORKSTATION
     VALUE: FieldItem = FIELD_COLLECTION.VALUE
     VALUE_LIST: FieldItem = FIELD_COLLECTION.VALUE_LIST
 
 
-class PolibasePersonInformationQuestError(Enum):
+class PolibasePersonInformationQuestStatus(Enum):
+    UNKNOWN: int = -1
+    GOOD: int = 0
     EMAIL_IS_EMPTY: int = 1
     EMAIL_IS_WRONG: int = 2
     EMAIL_IS_NOT_ACCESSABLE: int = 4
 
 
 class PolibasePersonVisitNotificationType(Enum):
     GREETING: int = auto()
@@ -968,15 +1104,15 @@
 
 class PASSWORD_GENERATION_ORDER:
 
     SPECIAL_CHARACTER: str = "s"
     LOWERCASE_ALPHABET: str = "a"
     UPPERCASE_ALPHABET: str = "A"
     DIGIT: str = "d"
-    DEFAULT_ORDER_LIST: List[str] = [SPECIAL_CHARACTER,
+    DEFAULT_ORDER_LIST: list[str] = [SPECIAL_CHARACTER,
                                      LOWERCASE_ALPHABET, UPPERCASE_ALPHABET, DIGIT]
 
 
 class PASSWORD:
 
     class SETTINGS:
 
@@ -1032,25 +1168,27 @@
 
 
 class ServiceCommands(Enum):
     ping: int = auto()
     subscribe: int = auto()
     unsubscribe: int = auto()
     unsubscribe_all: int = auto()
+    stop: int = auto()
     #Log
     send_log_message: int = auto()
     send_log_command: int = auto()
     send_message_to_user_or_workstation: int = auto()
+    add_message_to_queue: int = auto()
     send_delayed_message: int = auto()
     #Documents
     create_user_document: int = auto()
-    create_time_tracking_report: int = auto()
+    save_time_tracking_report: int = auto()
     create_barcodes_for_inventory: int = auto()
     create_barcode_for_polibase_person: int = auto()
-    create_barcode_for_polibase_person_card_registry_folder: int = auto()
+    create_qr_code: int = auto()
     check_inventory_report: int = auto()
     get_inventory_report: int = auto()
     save_inventory_report_item: int = auto()
     close_inventory_report: int = auto()
     #Polibase
     get_polibase_person_by_pin: int = auto()
     get_polibase_persons_by_pin: int = auto()
@@ -1151,14 +1289,27 @@
     get_storage_value: int = auto()
     #Resource Manager
     get_resource_status_list: int = auto()
     send_mobile_helper_message: int = auto()
 
     register_ct_indications_value: int = auto()
     get_last_ct_indications_value_list: int = auto()
+    #
+    test: int = auto()
+    #
+    execute_ssh_command: int = auto()
+    get_certificate_information: int = auto()
+    get_unix_free_space_information_by_drive_name: int = auto()
+    print_image: int = auto()
+    #
+    get_ogrn_value: int = auto()
+    get_fms_unit_name: int = auto()
+    #
+    start_polibase_person_information_quest: int = auto()
+
     
 
 class ServiceRoles(Enum):
 
     LOG: ServiceRoleDescription = ServiceRoleDescription(
                                             name="Log",
                                             description="Log service",
@@ -1176,21 +1327,30 @@
         host=CONST.HOST.WS255.NAME,
         port=CONST.RPC.PORT(),
         commands=[
             ServiceCommands.heat_beat
         ],
         modules=["schedule"])
 
+    INDICATIONS: ServiceRoleDescription = ServiceRoleDescription(
+        name="Indications",
+        description="Indications service",
+        host=CONST.HOST.WS255.NAME,
+        commands=[ServiceCommands.register_ct_indications_value,
+                  ServiceCommands.get_last_ct_indications_value_list
+                  ],
+        port=CONST.RPC.PORT(5),
+        modules=["fastapi", "uvicorn"]
+    )
+
     DATA_STORAGE: ServiceRoleDescription = ServiceRoleDescription(
                                             name="DataStorage",
                                             description="DataStorage service", 
                                             host=CONST.HOST.BACKUP_WORKER.NAME, 
                                             port=CONST.RPC.PORT(1),
-                                            auto_start=False,
-                                            auto_restart=False,
                                             commands=[
                                                         ServiceCommands.register_polibase_person_information_quest,
                                                         ServiceCommands.search_polibase_person_information_quests,
                                                         ServiceCommands.update_polibase_person_information_quest,
                                                         #
                                                         ServiceCommands.update_polibase_person_visit_to_data_stogare,
                                                         ServiceCommands.search_polibase_person_visits_in_data_storage,
@@ -1206,26 +1366,19 @@
                                                         ServiceCommands.set_settings_value,
                                                         #
                                                         ServiceCommands.search_polibase_person_notification_confirmation,
                                                         ServiceCommands.update_polibase_person_notification_confirmation,
                                                         #
                                                         ServiceCommands.get_storage_value,
                                                         ServiceCommands.set_storage_value,
+                                                        #
+                                                        ServiceCommands.get_ogrn_value,
+                                                        ServiceCommands.get_fms_unit_name
                                                     ],
-                                            modules=["mysql-connector-python", "pysos", "lmdbm"])
-
-    RESOURCE_MANAGER: ServiceRoleDescription = ServiceRoleDescription(
-        name="ResourceManager",
-        description="Resource Manager",
-        host=CONST.HOST.BACKUP_WORKER.NAME,
-        auto_start=False,
-        auto_restart=False,
-        commands=[ServiceCommands.get_resource_status_list],
-        modules=["paramiko"],
-        port=CONST.RPC.PORT(8))
+                                            modules=["mysql-connector-python", "pysos", "lmdbm", "dadata"])
 
     FILE_WATCHDOG: ServiceRoleDescription = ServiceRoleDescription(
         name="FileWatchdog",
         description="FileWatchdog service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
         port=CONST.RPC.PORT(2),
         modules=["watchdog"])
@@ -1300,24 +1453,24 @@
                                                 description="Documents service",
                                                 host=CONST.HOST.DC2.NAME,
                                                 port=CONST.RPC.PORT(1),
                                                 commands=
                                                         [
                                                             ServiceCommands.get_inventory_report,
                                                             ServiceCommands.create_user_document,
-                                                            ServiceCommands.create_time_tracking_report,
+                                                            ServiceCommands.save_time_tracking_report,
                                                             ServiceCommands.create_barcodes_for_inventory,
                                                             ServiceCommands.create_barcode_for_polibase_person,
-                                                            ServiceCommands.create_barcode_for_polibase_person_card_registry_folder,
+                                                            ServiceCommands.create_qr_code,
                                                             ServiceCommands.check_inventory_report,
                                                             ServiceCommands.save_inventory_report_item,
-                                                            ServiceCommands.close_inventory_report
+                                                            ServiceCommands.close_inventory_report,
                                                         ],
         modules=["xlsxwriter", "xlrd", "xlutils", "openpyxl",
-                                                    "python-barcode", "Pillow", "transliterate"]
+                                                    "python-barcode", "Pillow", "transliterate", "qrcode"]
                                             )
 
     PRINTER: ServiceRoleDescription = ServiceRoleDescription(
                                                     name="Printer",
                                                     description="Printer service", 
                                                     host=CONST.HOST.DC2.NAME, 
                                                     port=CONST.RPC.PORT(2),
@@ -1385,78 +1538,137 @@
         name="PolibaseDB",
         description="Polibase database api",
         host=CONST.HOST.POLIBASE.NAME,
         port=CONST.RPC.PORT(2),
         commands=[
                     ServiceCommands.create_polibase_database_backup
                 ],
-        modules=[])
+        )
 
     POLIBASE_APP: ServiceRoleDescription = ServiceRoleDescription(
         name="PolibaseApp",
         description="Polibase Application service",
         host=CONST.HOST.POLIBASE.NAME,
-        port=CONST.RPC.PORT(3),
-        commands=[],
-        modules=[])
+        port=CONST.RPC.PORT(3)
+        )
+
+    MESSAGE_QUEUE: ServiceRoleDescription = ServiceRoleDescription(
+        name="MessageQueue",
+        description="Message queue service",
+        host=CONST.HOST.BACKUP_WORKER.NAME,
+        port=CONST.RPC.PORT(100),
+        commands=[
+            ServiceCommands.add_message_to_queue
+        ]
+        )
 
-    MESSAGE: ServiceRoleDescription = ServiceRoleDescription(
-        name="Message",
+    POLIBASE_PERSON_NOTIFICATION: ServiceRoleDescription = ServiceRoleDescription(
+        name="PolibasePersonNotification",
+        description="Polibase Person Notification service",
+        host=CONST.HOST.BACKUP_WORKER.NAME,
+        port=CONST.RPC.PORT(7)
+        )
+    
+    POLIBASE_PERSON_INFORMATION_QUEST: ServiceRoleDescription = ServiceRoleDescription(
+        name="PolibasePersonInformationQuest",
+        description="Polibase Person Information Quest service",
+        host=CONST.HOST.BACKUP_WORKER.NAME,
+        port=CONST.RPC.PORT(10),
+         commands=[
+            ServiceCommands.start_polibase_person_information_quest
+        ]
+        )
+    
+    POLIBASE_PERSON_REVIEW_NOTIFICATION: ServiceRoleDescription = ServiceRoleDescription(
+        name="PolibasePersonReviewNotification",
+        description="Polibase Person Review Notification service",
+        host=CONST.HOST.BACKUP_WORKER.NAME,
+        port=CONST.RPC.PORT(11)
+        )
+    
+    MESSAGE_RECEIVER: ServiceRoleDescription = ServiceRoleDescription(
+        name="MessageReceiver",
         description="Message service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(6),
-        auto_start=False,
+        port=CONST.RPC.PORT(101),
         auto_restart=False,
-        commands=[
-            ServiceCommands.send_delayed_message
-        ],
         modules=["fastapi", "uvicorn"])
 
-    POLIBASE_NOTIFICATION: ServiceRoleDescription = ServiceRoleDescription(
-        name="PolibaseNotification",
-        description="Polibase Notification service",
+    SSH: ServiceRoleDescription = ServiceRoleDescription(
+        name="SSH",
+        description="Ssh service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(7),
+        port=CONST.RPC.PORT(9),
+        modules=["paramiko"],
+        commands=[ServiceCommands.execute_ssh_command,
+                  ServiceCommands.get_certificate_information,
+                  ServiceCommands.get_unix_free_space_information_by_drive_name]
+    )
+
+    WS_735: ServiceRoleDescription = ServiceRoleDescription(
+        name="ws_735",
+        description="ws-735 service",
+        host=CONST.HOST.WS735.NAME,
+        port=CONST.RPC.PORT(),
+        login="nak",
+        password="Soad7623!",
+        commands=[ServiceCommands.print_image],
+        modules=["pywin32", "Pillow"]
+    )
+
+    RECOGNIZE: ServiceRoleDescription = ServiceRoleDescription(
+        name="Recognize",
+        description="Recognize service",
+        host=CONST.HOST.WS255.NAME,
+        port=CONST.RPC.PORT(-2)
+    )
+
+    RECOGNIZE_TEST: ServiceRoleDescription = ServiceRoleDescription(
+        name="RecognizeTest",
+        description="Recognize test service",
+        host=CONST.HOST.WS255.NAME,
+        port=CONST.RPC.PORT(-3),
         auto_start=False,
         auto_restart=False,
-        commands=[],
-        modules=[])
+        visible_for_admin=False
+    )
+
+    CHECKER: ServiceRoleDescription = ServiceRoleDescription(
+        name="Checker",
+        description="Checker service",
+        host=CONST.HOST.BACKUP_WORKER.NAME,
+        commands=[ServiceCommands.get_resource_status_list],
+        port=CONST.RPC.PORT(8)
+    )
+
+    AUTOMATION: ServiceRoleDescription = ServiceRoleDescription(
+        name="Automation",
+        description="Automation service",
+        host=CONST.HOST.WS255.NAME,
+        port=CONST.RPC.PORT(-1)
+    )
 
     MOBILE_HELPER: ServiceRoleDescription = ServiceRoleDescription(
         name="MobileHelper",
         description="Mobile helper service",
         host=CONST.HOST.WS255.NAME,
-        auto_start=False,
-        auto_restart=False,
         commands=[ServiceCommands.send_mobile_helper_message],
         port=CONST.RPC.PORT(4)
-        )
-    
-    INDICATIONS: ServiceRoleDescription = ServiceRoleDescription(
-        name="Indications",
-        description="Indications service",
-        host=CONST.HOST.WS255.NAME,
-        auto_start=False,
-        auto_restart=False,
-        commands=[ServiceCommands.register_ct_indications_value,
-                  ServiceCommands.get_last_ct_indications_value_list],
-        port=CONST.RPC.PORT(5)
     )
-    
-#####################################################################################################
 
     DEVELOPER: ServiceRoleDescription = ServiceRoleDescription(
         name="Developer",
         description="Developer service",
         host=CONST.HOST.DEVELOPER.NAME,
-        port=CONST.RPC.PORT(),
-        visible_for_admin = False,
-        auto_restart = False,
+        port=CONST.RPC.PORT(1),
+        visible_for_admin=False,
         auto_start=False,
-        weak_subscribtion = True)
+        auto_restart=False,
+        commands=[ServiceCommands.test]
+    )
 
 class SubscribtionTypes:
     BEFORE: int = 1
     AFTER: int = 2
 
 class WorkstationMessageMethodTypes(Enum):
 
@@ -1467,15 +1679,15 @@
 class MessageTypes(Enum):
 
     WHATSAPP: int = 1
     TELEGRAM: int = 2
     INTERNAL: int = 3
 
 
-class MessageStatus(Enum):
+class MessageStatuses(Enum):
 
     REGISTERED: int = 0
     COMPLETE: int = 1
     AT_WORK: int = 2
     ERROR: int = 3
     ABORT: int = 4
 
@@ -1495,33 +1707,46 @@
 106 - предварительно
 107 - подверждено
 108 - оказано
 109 к оплате
 """
 
 class SETTINGS(Enum):
+
+    VALENTA_SYNCHRONIZATION_TEST: SettingsValue = SettingsValue(None, False)
+
+    CT_TEMPERATURE_CORRECTION: SettingsValue = SettingsValue(None, 0.7)
+
+    HOSPITAL_WORK_DAY_START_TIME: SettingsValue = SettingsValue(None, "8:00")
+    HOSPITAL_WORK_DAY_END_TIME: SettingsValue = SettingsValue(None, "20:00")
+    OFFICE_WORK_DAY_START_TIME: SettingsValue = SettingsValue(None, "8:30")
+    OFFICE_WORK_DAY_END_TIME: SettingsValue = SettingsValue(None, "17:00")
+
+
+    INDICATION_CT_NOTIFICATION_START_TIME: SettingsValue = SettingsValue(None, ["8:00", "17:00"])
+
+    USER_USE_CACHE: SettingsValue = SettingsValue(None, 1)
     
-    POLIBASE_PERSON_INFORMATION_QUEST_IS_ON: SettingsValue = SettingsValue(
-        None, False)
+    POLIBASE_PERSON_INFORMATION_QUEST_IS_ON: SettingsValue = SettingsValue(None, True)
     #
-    POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON: SettingsValue = SettingsValue(None, False)
+    POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON: SettingsValue = SettingsValue(None, True)
 
     POLIBASE_PERSON_REVIEW_NOTIFICATION_DAY_DELTA: SettingsValue = SettingsValue(None, 1)
 
     POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION: SettingsValue = SettingsValue(
         None, CONST.POLIBASE.PERSON_REVIEW_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION)
 
     POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT: SettingsValue = SettingsValue(
         None, CONST.POLIBASE.PERSON_REVIEW_NOTIFICATION_TEXT)
 
-    POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME: SettingsValue = SettingsValue(None, "13:00")
+    POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME: SettingsValue = SettingsValue(None, "13:53")
     #
     RESOURCE_MANAGER_CHECK_SITE_CERTIFICATE_START_TIME: SettingsValue = SettingsValue(None, "8:00")
     #
-    POLIBAE_CREATION_DB_DUMP_START_TIME: SettingsValue = SettingsValue(None, "20:30")
+    POLIBASE_CREATION_DB_DUMP_START_TIME: SettingsValue = SettingsValue(None, "20:30")
     #
     RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES: SettingsValue = SettingsValue(None, 15)
     #
     POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE_FOR_CONFIRMED_NOTIFICATION: SettingsValue = SettingsValue(
         None, CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION + CONST.POLIBASE.SEND_TELEGRAM_BOT_TEXT)
 
     POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE: SettingsValue = SettingsValue(
@@ -1571,15 +1796,15 @@
     
     POLIBASE_PERSON_VISIT_NOTIFICATION_TEST_TELEPHONE_NUMBER: SettingsValue = SettingsValue(
         None, "+79146717744")
 
     POLIBASE_PERSON_REVIEW_NOTIFICATION_TEST_TELEPHONE_NUMBER: SettingsValue = SettingsValue(
         None, None)
     
-    WHATSAPP_FUNCTIONAL_IS_ON: SettingsValue = SettingsValue(
+    WHATSAPP_SENDING_MESSAGES_VIA_WAPPI_IS_ON: SettingsValue = SettingsValue(
         None, True)
     
     WHATSAPP_BUFFERED_MESSAGE_MIN_DELAY_IN_MILLISECONDS: SettingsValue = SettingsValue(
         None, 6000)
     
     WHATSAPP_BUFFERED_MESSAGE_MAX_DELAY_IN_MILLISECONDS: SettingsValue = SettingsValue(
         None, 12000)
@@ -1589,31 +1814,35 @@
 
     MOBILE_HELPER_USER_DATA_INPUT_TIMEOUT: SettingsValue = SettingsValue(
         None, CONST.MOBILE_HELPER.USER_DATA_INPUT_TIMEOUT)
     
     POLIBASE_WAS_EMERGENCY_CLOSED_NOTIFICATION_TEXT: SettingsValue = SettingsValue(
         None, "к сожалениию наш Полибейс поломался и был аварийно закрыт, ожидайте сообщение о просьбе переоткрыть его!")
     
-    WORKSTATION_SHUTDOWN_TIME: SettingsValue = SettingsValue(None, "23:04")
-    WORKSTATION_REBOOT_TIME: SettingsValue = SettingsValue(None, "21:37")
+    POLIBASE_WAS_RESTARTED_NOTIFICATION_TEXT: SettingsValue = SettingsValue(
+        None, "Полибейс перезагружен, можете переоткрыть его.")
+    
+    WORKSTATION_SHUTDOWN_TIME: SettingsValue = SettingsValue(None, "21:00")
+
+    WORKSTATION_REBOOT_TIME: SettingsValue = SettingsValue(None, "21:00")
 
 
 class LogCommands(Enum):
 
     DEBUG: LogCommandDescription = LogCommandDescription(
         "It is a debug command", LogChannels.NOTIFICATION, LogLevels.DEBUG.value)
         
     PRINTER_REPORT: LogCommandDescription = LogCommandDescription("Принтер {printer_name} ({location}):\n {printer_report}", LogChannels.PRINTER, LogLevels.NORMAL.value, (ParamItem(
         "printer_name", "Name of printer"), ParamItem("location", "Location"), ParamItem("printer_report", "Printer report")))
     #
     LOG_IN: LogCommandDescription = LogCommandDescription(
-        "Пользователь {full_name} ({login}) вошел с компьютера {computer_name}", LogChannels.SERVICE, LogLevels.NORMAL.value, (ParamItem("full_name", "Name of user"), ParamItem("login", "Login of user"), ParamItem("computer_name", "Name of computer")))
+        "Пользователь {full_name} ({login}) вошел с компьютера {computer_name}", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("full_name", "Name of user"), ParamItem("login", "Login of user"), ParamItem("computer_name", "Name of computer")))
 
     SESSION_STARTED: LogCommandDescription = LogCommandDescription(
-        "Пользователь {full_name} ({login}) начал пользоваться программой {app_name}.\nВерсия: {version}.\nНазвание компьютера: {computer_name}", LogChannels.SERVICE, LogLevels.NORMAL.value, (ParamItem("full_name", "Name of user"), ParamItem("login", "Login of user"), ParamItem("app_name", "Name of user"),  ParamItem("version", "Version"), ParamItem("computer_name", "Name of computer")))
+        "Пользователь {full_name} ({login}) начал пользоваться программой {app_name}.\nВерсия: {version}.\nНазвание компьютера: {computer_name}", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("full_name", "Name of user"), ParamItem("login", "Login of user"), ParamItem("app_name", "Name of user"),  ParamItem("version", "Version"), ParamItem("computer_name", "Name of computer")))
 
     SERVICE_STARTS: LogCommandDescription = LogCommandDescription(
         "Сервис {service_name} ({service_description}) запускается!\nИмя хоста: {host_name}\nПорт: {port}\nИдентификатор процесса: {pid}\n", LogChannels.SERVICE, LogLevels.SILENCE.value, (ParamItem("service_name", "Name of service"), ParamItem("service_description", "Description of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("pid", "PID")))
     
     SERVICE_STARTED: LogCommandDescription = LogCommandDescription(
         "Сервис {service_name} ({service_description}) запущен!\nИмя хоста: {host_name}\nПорт: {port}\nИдентификатор процесса: {pid}\n", LogChannels.SERVICE, LogLevels.NORMAL.value, (ParamItem("service_name", "Name of service"), ParamItem("service_description", "Description of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("pid", "PID")))
     
@@ -1621,14 +1850,32 @@
         "Сервис {service_name} ({service_description}) не запущен!\nИмя хоста: {host_name}\nПорт: {port}\nОшибка:{error}", LogChannels.SERVICE, LogLevels.ERROR.value, (ParamItem("service_name", "Name of service"), ParamItem("service_description", "Description of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("error", "Error")))
 
     SERVICE_IS_INACCESIBLE_AND_WAITING_TO_BE_RESTARTED: LogCommandDescription = LogCommandDescription(
         "Сервис {service_name} ({service_description}) недоступен и будет перезапущен!\nИмя хоста: {host_name}\nПорт: {port}\nИдентификатор процесса: {pid}\n", LogChannels.SERVICE, LogLevels.ERROR.value, (ParamItem("service_name", "Name of service"), ParamItem("service_description", "Description of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("pid", "PID")))
  
     WHATSAPP_MESSAGE_RECEIVED: LogCommandDescription = LogCommandDescription(
         "Получено сообщение", LogChannels.NOTIFICATION, LogLevels.SILENCE.value, (ParamItem("message", "Сообщение"),))
+    
+    NEW_FILE_DETECTED: LogCommandDescription = LogCommandDescription(
+        "Новый файл", LogChannels.IT, LogLevels.SILENCE.value, (ParamItem("path", "Путь к файлу"),))
+    
+    NEW_POLIBASE_DOCUMENT_DETECTED: LogCommandDescription = LogCommandDescription(
+        "Новый Polibase документ", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("path", "Путь к файлу"), ParamItem("person_pin", "Идентификационный номер пациента"), ParamItem("document_name", "Имя документа")))
+
+    COMPUTER_WAS_STARTED: LogCommandDescription = LogCommandDescription(
+        "Компьютер {name} загрузился", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("name", "Название компьютера"),))
+    
+    SERVER_WAS_STARTED: LogCommandDescription = LogCommandDescription(
+        "Сервер {name} загрузился", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("name", "Название сервера"),))
+    
+    RESOURCE_INACCESSABLE: LogCommandDescription = LogCommandDescription(
+        "Ресурс {resource_name} недоступен. {reason_string}", LogChannels.RESOURCES, LogLevels.ERROR.value, (ParamItem("resource_name", "Название ресурса"), ParamItem("resource", "Ресурс"), ParamItem("at_first_time", "Признак первого раза"), ParamItem("reason_string", "Строка причины"), ParamItem("reason", "Причины")))
+    
+    RESOURCE_ACCESSABLE: LogCommandDescription = LogCommandDescription(
+        "Ресурс {resource_name} доступен", LogChannels.RESOURCES, LogLevels.NORMAL.value, (ParamItem("resource_name", "Название ресурса"), ParamItem("resource", "Ресурс"), ParamItem("at_first_time", "Признак первого раза")))
 
     #
     BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_STARTED: LogCommandDescription = LogCommandDescription(
         "Robocopy: Начато выполнение задания: {status}", LogChannels.BACKUP, LogLevels.NOTIFICATION.value, (ParamItem("status", ""),))
 
     BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_COMPLETED: LogCommandDescription = LogCommandDescription(
         "Robocopy: Завершено выполнение задания: {status}", LogChannels.BACKUP, LogLevels.NOTIFICATION.value, (ParamItem("status", ""),))
```

### Comparing `pih-1.421/pih/pih.py` & `pih-1.43/pih/pih.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,49 +9,84 @@
 import dataclasses
 import importlib.util
 import locale
 import os
 import platform
 import json
 import pkg_resources
-import requests
 import re
 import subprocess
 from subprocess import DEVNULL, STDOUT, CompletedProcess
 import sys
-from typing import Any, Callable, List, Tuple
+from typing import Any, Callable, Tuple
 import colorama
 from colorama import Back, Style, Fore
 from prettytable import PrettyTable
 import requests
 from requests import ConnectTimeout, Response
 import traceback
 from contextlib import contextmanager
+import base64
+import uuid
 
 try:
     from packaging.version import parse
 except ImportError:
     from pip._vendor.packaging.version import parse
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
-from pih.tools import DataTool, EnumTool, PathTool, ResultTool, FullNameTool, PasswordTools, ResultUnpack, DateTimeTool, BitMask as BM, ParameterList
-from pih.collection import ActionValue, T, FieldItem, FieldItemList, FullName, InventoryReportItem, LogCommandDescription, LoginPasswordPair, Mark, MarkDivision, MarkGroup, MarkGroupStatistics, ParamItem, PasswordSettings, PolibasePerson, PrinterADInformation, PrinterReport, PrinterStatus, Result, ServiceRoleInformation, ServiceRoleDescription, TemporaryMark, TimeTrackingEntity, TimeTrackingResultByDate, TimeTrackingResultByDivision, TimeTrackingResultByPerson, User, UserContainer, Workstation, WhatsAppMessage, WhatsAppMessageListPayload, WhatsAppMessageButtonsPayload, WorkstationDescription, SettingsValue, PolibasePersonVisitDS, PolibasePersonVisitNotification, PolibasePersonVisitNotificationDS, DelayedMessage, MessageSearchCritery, DelayedMessageDS, PolibasePersonInformationQuest, PolibasePersonVisitSearchCritery, RobocopyJobStatus, PolibasePersonNotificationConfirmation, ResourceDescription, ResourceStatus, SiteResourceStatus, CTIndicationDS, CTIndicationValue
-from pih.const import CONST, FIELD_NAME_COLLECTION, FIELD_COLLECTION, FILE, PASSWORD, PATHS, USER_PROPERTY, WorkstationMessageMethodTypes, LogChannels, LogCommands, LogLevels, MarkType, ServiceCommands, ServiceRoles, SETTINGS, MessageTypes, MessageStatus, RESOURCE_DESCRIPTION_COLLECTION, CheckableSections
+from pih.tools import DataTool, EnumTool, PathTool, ResultTool, FullNameTool, PasswordTools, ResultUnpack, DateTimeTool, BitMask as BM, ParameterList, StringTool, ListTool, NetworkTool
+from pih.collection import ActionValue, T, FieldItem, FieldItemList, FullName, InventoryReportItem, LogCommandDescription, LoginPasswordPair, Mark, MarkDivision, MarkGroup, MarkGroupStatistics, ParamItem, PasswordSettings, PolibasePerson, PrinterADInformation, PrinterReport, PrinterStatus, Result, ServiceRoleInformation, ServiceRoleDescription, TemporaryMark, TimeTrackingEntity, TimeTrackingResultByDate, TimeTrackingResultByDivision, TimeTrackingResultByPerson, User, UserContainer, Workstation, WhatsAppMessage, WhatsAppMessageListPayload, WhatsAppMessageButtonsPayload, WorkstationDescription, SettingsValue, PolibasePersonVisitDS, PolibasePersonVisitNotification, PolibasePersonVisitNotificationDS, DelayedMessage, MessageSearchCritery, DelayedMessageDS, PolibasePersonInformationQuest, PolibasePersonVisitSearchCritery, RobocopyJobStatus, PolibasePersonNotificationConfirmation, ResourceDescription, ResourceStatus, SiteResourceStatus, CTIndicationItem, CTIndicationValue, PolibaseScannedDocument, OGRN, Message
+from pih.const import CONST, URLS, DATA, FIELD_NAME_COLLECTION, FIELD_COLLECTION, FILE, FIELD_COLLECTION_ALIAS, PASSWORD, PATHS, HOSTS, USER_PROPERTY, WorkstationMessageMethodTypes, LogChannels, LogCommands, LogLevels, MarkType, ServiceCommands, ServiceRoles, SETTINGS, MessageTypes, MessageStatuses, RESOURCE, CheckableSections, AD, MEDICAl_DOCUMENT, FONT
 from pih.rpc_collection import Subscriber
 from pih.rpc import RPC, Error, SubscribtionTypes
 
+class IClosable:
+
+    def close() -> None:
+        raise NotImplemented()
+
+class ServiceListener:
+    
+    def __init__(self):
+        self.service: RPC.Service | None = None
+        self.service_command_list: list[ServiceCommands] = None
+        self.host: str = A.OS.host()
+        self.port: int = NetworkTool.next_free_port()
+
+    def listen_for(self, service_command_list: list[ServiceCommands], handler: Callable[[str, ParameterList, IClosable], Any]) -> None:     
+        self.service_command_list = service_command_list
+  
+        def service_started_handler(service: RPC.Service) -> None:
+            self.service = service
+            for service_command in service_command_list:
+                service.subscribe_on(service_command)
+
+        service_description: ServiceRoleDescription = ServiceRoleDescription(
+            name=f"Subscriber_{self.host}_{ self.port}",
+            description="Subscriber",
+            host=self.host,
+            port=self.port,
+            weak_subscribtion=True)
+        
+        PIH.SERVICE.ADMIN.serve(service_description, lambda command_name, parameter_list, _: handler(command_name, parameter_list, self), False, service_started_handler)
+        
+    def close(self) -> None:
+        self.service.unsubscribe(self.service_command_list)
+        self.service.stop()    
+
 
 class MarkOutputAbstract:
 
     def by_any(self, value: str) -> None:
         raise NotImplemented()
 
-    def result(self, result: Result[List[Mark]], caption: str, use_index: bool = False) -> None:
+    def result(self, result: Result[list[Mark]], caption: str, use_index: bool = False) -> None:
         raise NotImplemented()
 
 class OutputAbstract:
     
     def indent(self, count: int = 1) -> None:
         raise NotImplemented()
     
@@ -192,15 +227,15 @@
 
     def bright_str(self, text: str, text_before: str = None, text_after: str = None) -> str:
         raise NotImplemented()
 
     def get_number(self, value: int) -> str:
         raise NotImplemented()
 
-    def write_result(self, result: Result[T], use_index: bool = True, item_separator: str = "\n", empty_result_text: str = "Не найдено", separated_result_item: bool = True, label_function:  Callable[[Any], str] = None, data_label_function: Callable[[int, FieldItem, Result[T], Any], Tuple[bool, str]] = None, title: str = None) -> None:
+    def write_result(self, result: Result[T], use_index: bool = True, item_separator: str = "\n", empty_result_text: str = "Не найдено", separated_result_item: bool = True, label_function:  Callable[[Any, int], str] = None, data_label_function: Callable[[int, FieldItem, Result[T], Any], Tuple[bool, str]] = None, title: str = None) -> None:
         raise NotImplemented()
 
     @contextmanager
     def send_to_group(self, group: CONST.MESSAGE.WHATSAPP.GROUP) -> bool:
         raise NotImplemented()
 
 class MarkOutputBase(MarkOutputAbstract):
@@ -208,38 +243,42 @@
     def __init__(self):
         self.parent: OutputBase
 
 
 class MarkOutput(MarkOutputBase):
 
     def by_any(self, value: str) -> None:
-        self.result(
-            PIH.RESULT.MARK.by_any(value), "Найденные карты доступа:", True)
+        try:
+            self.result(PIH.RESULT.MARK.by_any(value) , "Найденные карты доступа:", True)
+        except NotFound as error:
+            self.parent.error(error.get_details())
+
+           
 
-    def result(self, result: Result[List[Mark]], caption: str, use_index: bool = False) -> None:
+    def result(self, result: Result[list[Mark]], caption: str, use_index: bool = False) -> None:
         self.parent.table_with_caption_first_title_is_centered(result, caption, use_index)
 
 
 class UserOutputAbstract:
 
-    def result(self, result: Result[List[User]], caption: str = None, use_index: bool = False, root_location: str = CONST.AD.ACTIVE_USERS_CONTAINER_DN) -> None:
+    def result(self, result: Result[list[User]], caption: str = None, use_index: bool = False, root_location: str = AD.ACTIVE_USERS_CONTAINER_DN) -> None:
         raise NotImplemented()
 
-    def get_formatted_given_name(self, value: str) -> str:
+    def get_formatted_given_name(self, value: str | None = None) -> str:
         return value
 
 class OutputExtendedAbstract:
 
     def pih_title(self) -> None:
         raise NotImplemented()  
 
     def rpc_service_header(self, host: str, port: int, description: str) -> None:
         raise NotImplemented()  
 
-    def service_header(self, role: ServiceRoles) -> None:
+    def service_header(self, service_role_description: ServiceRoleDescription) -> None:
         raise NotImplemented()  
 
     def free_marks(self, show_guest_marks: bool, use_index: bool = False) -> None:
         raise NotImplemented()  
 
     def guest_marks(self, use_index: bool = False) -> None:
         raise NotImplemented()
@@ -275,38 +314,44 @@
         raise NotImplemented()  
 
     def template_users_for_result(self, data: dict, use_index: bool = False) -> None:
         raise NotImplemented()  
 
     def clear_screen(self) -> None:
         raise NotImplemented()
+    
+    def write_video(self, caption: str, video_content: str) -> None:
+            raise NotImplemented()
+
+    def write_image(self, caption: str, image_content: str) -> None:
+        raise NotImplemented()
 
 class UserOutputBase(UserOutputAbstract):
 
     def __init__(self):
         self.parent: OutputBase
 
 class UserOutput(UserOutputBase):
 
-    def result(self, result: Result[List[User]], caption: str = None, use_index: bool = False, root_location: str = CONST.AD.ACTIVE_USERS_CONTAINER_DN) -> None:
+    def result(self, result: Result[list[User]], caption: str = None, use_index: bool = False, root_location: str = AD.ACTIVE_USERS_CONTAINER_DN) -> None:
         data: list = DataTool.as_list(result.data)
         fields: FieldItemList = result.fields
         base_location_list = PIH.DATA.FORMAT.location_list(
             root_location, False)
         root_base_location = base_location_list[0:2]
         root_base_location.reverse()
-        base_location = CONST.AD.LOCATION_JOINER.join([".".join(
-            root_base_location), CONST.AD.LOCATION_JOINER.join(base_location_list[2:])])
+        base_location = AD.LOCATION_JOINER.join([".".join(
+            root_base_location), AD.LOCATION_JOINER.join(base_location_list[2:])])
         location_field = fields.get_item_by_name(
             FIELD_NAME_COLLECTION.DN)
         pevious_caption: str = location_field.caption
         location_field.caption = f"{location_field.caption} ({base_location})"
         def modify_data(field: FieldItem, user: User) -> str:
             if field.name == USER_PROPERTY.DN:
-                return CONST.AD.LOCATION_JOINER.join(filter(
+                return AD.LOCATION_JOINER.join(filter(
                     lambda x: x not in base_location_list, PIH.DATA.FORMAT.location_list(user.distinguishedName)))
             if field.name == USER_PROPERTY.USER_ACCOUNT_CONTROL:
                 return "\n".join(PIH.DATA.FORMAT.get_user_account_control_values(user.userAccountControl))
             if field.name == USER_PROPERTY.DESCRIPTION:
                 return user.description
             if field.name == USER_PROPERTY.NAME:
                 return "\n".join(user.name.split(" "))
@@ -317,15 +362,15 @@
 
 
 class InputAbstract:
 
     def input(self, caption: str = None, new_line: bool = True, check_function: Callable[[str], str] = None) -> str:
         raise NotImplemented()
 
-    def card_registry_folder(self) -> str:
+    def polibase_person_card_registry_folder(self) -> str:
         raise NotImplemented()
 
     def telephone_number(self, format: bool = True, telephone_prefix: str = CONST.TELEPHONE_NUMBER_PREFIX) -> str:
         raise NotImplemented()
 
     def email(self) -> str:
         raise NotImplemented()
@@ -335,24 +380,24 @@
 
     def description(self) -> str:
         raise NotImplemented()
 
     def login(self, check_on_exists: bool = False) -> str:
         raise NotImplemented()
 
-    def indexed_list(self, caption: str, name_list: List[Any], caption_list: List[str], by_index: bool = False) -> str:
+    def indexed_list(self, caption: str, name_list: list[Any], caption_list: list[str], by_index: bool = False) -> str:
         raise NotImplemented()
 
     def indexed_field_list(self, caption: str, list: FieldItemList) -> str:
         raise NotImplemented()
 
-    def index(self, caption: str, data: List, label_function: Callable[[Any, int], str] = None, use_zero_index: bool = False) -> int:
+    def index(self, caption: str, data: list, label_function: Callable[[Any, int], str] = None, use_zero_index: bool = False) -> int:
         raise NotImplemented()
 
-    def item_by_index(self, caption: str, data: List[Any], label_function: Callable[[Any, int], str] = None, use_zero_index: bool = False) -> Any:
+    def item_by_index(self, caption: str, data: list[Any], label_function: Callable[[Any, int], str] = None, use_zero_index: bool = False) -> Any:
         raise NotImplemented()
 
     def tab_number(self, check: bool = True) -> str:
         raise NotImplemented()
 
     def password(self, secret: bool = True, check: bool = False, settings: PasswordSettings = None, is_new: bool = True) -> str:
         raise NotImplemented()
@@ -362,36 +407,36 @@
 
     def name(self) -> str:
         raise NotImplemented()
 
     def full_name(self, one_line: bool = False) -> FullName:
         raise NotImplemented()
 
-    def yes_no(self, text: str = " ", enter_for_yes: bool = False, yes_label: str = None, no_label: str = None) -> bool:
+    def yes_no(self, text: str = " ", enter_for_yes: bool = False, yes_label: str = None, no_label: str = None, yes_checker: Callable[[str], bool] = None) -> bool:
         raise NotImplemented()
 
     def message_for_user_by_login(self, login: str) -> str:
         raise NotImplemented()
 
-    def polibase_person_any(self) -> str:
+    def polibase_person_any(self, title: str | None = None) -> str:
         raise NotImplemented()
 
 
 class UserInputAbstract:
 
     def container(self) -> UserContainer:
         raise NotImplemented()
 
     def by_name(self) -> User:
         raise NotImplemented()
 
     def title_any(self, title: str = None) -> str:
         raise NotImplemented()
 
-    def by_any(self, value: str = None, active: bool = None, title: str = None, use_all: bool = False) -> List[User]:
+    def by_any(self, value: str = None, active: bool = None, title: str = None, use_all: bool = False) -> list[User]:
         raise NotImplemented()
 
     def telephone_number(self, value: str = None, active: bool = None, title: str = None) -> User:
         raise NotImplemented()
 
     def template(self) -> dict:
         raise NotImplemented()
@@ -408,15 +453,15 @@
     def generate_password(self, once: bool = False, settings: PasswordSettings = PASSWORD.SETTINGS.DEFAULT) -> str:
         raise NotImplemented()
 
 
 class UserInputBase(UserInputAbstract):
 
     def __init__(self):
-        self.parent: InputBase
+        self.parent: InputBase = None
 
 
 class MarkInputAbstract:
 
     def free(self, group: MarkGroup = None) -> Mark:
         raise NotImplemented()
 
@@ -454,14 +499,15 @@
         self.TEXT_AFTER: str = ""
         self.INDEX: str = "  "
         self.INDEX_COUNT: int = 0
         self.user: UserOutputBase = user_output
         self.user.parent = self
         self.mark: MarkOutputBase = mark_output
         self.mark.parent = self
+        self.personalize = False
 
 
 class SessionAbstract:
 
     def run_forever_untill_enter_not_pressed(self) -> None:
         raise NotImplemented()
 
@@ -480,15 +526,15 @@
     def start(self, login: str, notify: bool = True) -> None:
         raise NotImplemented()
 
     def say_hello(self) -> None:
         raise NotImplemented()
     
     @property
-    def argv(self) -> List[str]:
+    def argv(self) -> list[str]:
         raise NotImplemented()
 
     def arg(self, index: int = None, default_value: str = None) -> str:
         raise NotImplemented()
 
     def get_file_path(self) -> str:
         raise NotImplemented()
@@ -496,27 +542,27 @@
     @property
     def file_name(self) -> str:
         raise NotImplemented()
 
     def authenticate(self, exit_on_fail: bool = True) -> bool:
         raise NotImplemented()
 
-    def add_allowed_group(self, value: CONST.AD.Groups) -> None:
+    def add_allowed_group(self, value: AD.Groups) -> None:
         raise NotImplemented()
 
 class SessionBase(SessionAbstract):
 
     def __init__(self, input: InputBase = None, output: OutputBase = None):
-        self.allowed_groups: List[CONST.AD.Groups] = []
+        self.allowed_groups: list[AD.Groups] = []
         self.login: str = None
         self.user: User = None
         self.input: InputBase = input
         self.output: OutputBase = output
 
-    def add_allowed_group(self, value: CONST.AD.Groups) -> None:
+    def add_allowed_group(self, value: AD.Groups) -> None:
         self.allowed_groups.append(value)
 
 
 class Session(SessionBase):
 
     def __init__(self, input: InputBase = None, output: OutputBase = None):
         super().__init__(input, output)
@@ -564,15 +610,15 @@
             self.output.good(f"Добро пожаловать, {user.name}")
             self.output.new_line()
             return
         self.output.error(f"Ты кто такой? Давай, до свидания...")
         self.exit()
 
     @property
-    def argv(self) -> List[str]:
+    def argv(self) -> list[str]:
         return sys.argv[1:] if len(sys.argv) > 1 else None
     
     def arg(self, index: int = 0, default_value: Any = None) -> str:
         return DataTool.by_index(self.argv, index, default_value)
 
     def get_file_path(self) -> str:
         return sys.argv[0]
@@ -586,15 +632,15 @@
             if once and self.authenticated:
                 return True
             self.output.green("Инициализация...")
             self.output.clear_screen()
             self.output.pih_title()
             if PIH.SERVICE.check_accessibility(ServiceRoles.AD): 
                 login: str = PIH.OS.get_login()
-                self.output.head1(f"{FullNameTool.to_given_name(A.R_U.by_login(login).data.name)}, пожалуйста, пройдите аутентификацию...")
+                self.output.head1(f"{FullNameTool.to_given_name(A.R_U.by_login(login, cached=False).data.name)}, пожалуйста, пройдите аутентификацию...")
                 self.output.new_line()
                 if not self.input.yes_no(f"Использовать логин '{login}'", True):
                     login = PIH.input.login()
                 password: str = PIH.input.password(is_new=False)
                 if DataTool.rpc_unrepresent(RPC.call(ServiceCommands.authenticate, (login, password))):
                     self.authenticated = True
                     self.start(login, False)
@@ -635,15 +681,15 @@
 class Output(OutputBase):
 
     def indent(self, count: int = 1) -> None:
         self.INDEX_COUNT = count
         self.TEXT_BEFORE = self.INDEX*count
 
     def bold(self, value: str) -> str:
-        return self.text_color(Fore.LIGHTCYAN_EX, value)
+        return self.text_color(Fore.RED, value)
 
     def italic(self, value: str) -> str:
         return value
 
     def reset_indent(self) -> None:
         self.TEXT_BEFORE = ""
 
@@ -668,18 +714,22 @@
     def color(self, color: int, text: str, text_before: str = None, text_after: str = None) -> None:
         self.write_line(self.color_str(
             color, text, text_before, text_after))
 
     def write_line(self, text: str) -> None:
         print(text)
 
+    @contextmanager
+    def personalized(self) -> bool:
+        pass
+
     def index(self, index: int, text: str, max_index: int = None) -> None:
         indent: str = ""
         if max_index is not None:
-            indent = " " * (len(str(max_index)) - len(str(index)))
+            indent = " " * 2 * (len(str(max_index)) - len(str(index)))
         if index is None:
             self.write_line(f"{indent}{text}")
         else:
             self.write_line(f"{index}. {indent}{text}")
 
     def input(self, caption: str) -> None:
         self.write_line(self.input_str(
@@ -798,15 +848,15 @@
 
     def get_number(self, value: int) -> str:
         return CONST.VISUAL.NUMBER_SYMBOLS[value - 1]
 
     def header(self, caption: str) -> None:
         self.head2(caption)
 
-    def write_result(self, result: Result[T], use_index: bool = True, item_separator: str = "\n", empty_result_text: str = "Не найдено", separated_result_item: bool = True, label_function: Callable[[Any], str] = None, data_label_function: Callable[[int, FieldItem, Result, Any], Tuple[bool, str]] = None, title: str = None) -> None:
+    def write_result(self, result: Result[T], use_index: bool = True, item_separator: str = "\n", empty_result_text: str = "Не найдено", separated_result_item: bool = True, label_function: Callable[[Any, int], str] = None, data_label_function: Callable[[int, FieldItem, Result, Any], Tuple[bool, str]] = None, title: str = None) -> None:
         data: list = DataTool.as_list(result.data)
         result_string_list: list[str] = None
         if DataTool.is_empty(data):
             self.new_line()
             self.write_line(empty_result_text)
         else:
             if not DataTool.is_empty(title):
@@ -821,15 +871,15 @@
                         if not field.visible:
                             continue
                         item_data_value: str = None
                         if isinstance(data_item, dict):
                             item_data_value = data_item[field.name]
                         elif dataclasses.is_dataclass(data_item):
                             item_data_value = data_item.__getattribute__(field.name)
-                        item_data_value = item_data_value if DataTool.is_empty(item_data_value) else field.data_formatter.format(data=item_data_value)
+                        item_data_value = item_data_value if DataTool.is_empty(item_data_value) else PIH.DATA.FORMAT.by_name(field.data_formatter, item_data_value) or field.data_formatter.format(data=item_data_value) 
                         if DataTool.is_empty(item_data_value):
                             if data_label_function is None:
                                 continue
                         default_value_label_function: Callable[[int, FieldItem, Result[T], Any], (
                             bool, str)] = lambda _1, field, _2, data_value: (True, f"{self.bold(field.caption)}: {data_value}")
                         result_data_label_function: Callable[[int, FieldItem, Result[T], Any], (bool, str)] = data_label_function or default_value_label_function 
                         label_value_result: tuple[bool, str] = result_data_label_function(index, field, data_item, item_data_value)
@@ -839,15 +889,15 @@
                             if label_value is None and field.default_value is not None:
                                 label_value = field_item.default_value
                         else:
                             label_value = default_value_label_function(index, field, data_item, item_data_value)[1]
                         if not DataTool.is_empty(label_value):
                             result_string_list.append(label_value)
                 else:
-                    result_string_list.append(label_function(data_item))  
+                    result_string_list.append(label_function(data_item, index))  
                 if separated_result_item:
                     self.separated_line()
                 self.write_line(item_separator.join(result_string_list))
 
     def clear_screen(self):
         os.system('cls' if os.name == 'nt' else 'clear')
 
@@ -863,35 +913,34 @@
         self.blue("PIH service")
         self.blue(f"Version: {PIH.VERSION.local()}")
         self.blue(f"PyPi Version: {PIH.VERSION.remote()}")
         self.green(f"Service host: {host}")
         self.green(f"Service port: {port}")
         self.green(f"Service name: {description}")
 
-    def service_header(self, role: ServiceRoles) -> None:
-        service_role_value: ServiceRoleDescription = role.value
-        if service_role_value.isolated:
+    def service_header(self, service_role_description: ServiceRoleDescription) -> None:
+        if service_role_description.isolated:
             self.blue(f"[Isolate]")
         self.blue("Запуск сервиса")
         self.blue(f"PIH версия: {PIH.VERSION.remote()}")
-        self.green(f"Хост: {service_role_value.host}")
-        self.green(f"Порт: {service_role_value.port}")
-        self.green(f"Имя сервиса: {service_role_value.name}")
+        self.green(f"Хост: {service_role_description.host}")
+        self.green(f"Порт: {service_role_description.port}")
+        self.green(f"Имя сервиса: {service_role_description.name}")
         self.green(
-            f"Описание сервиса: {service_role_value.description}")
+            f"Описание сервиса: {service_role_description.description}")
         self.green(
-            f"Идентификатор процесса: {service_role_value.pid}")
+            f"Идентификатор процесса: {service_role_description.pid}")
 
     def free_marks(self, show_guest_marks: bool, use_index: bool = False, sort_by_tab_number: bool = True) -> None:
         def sort_function(item: Mark) -> Any:
             return item.TabNumber if sort_by_tab_number else item.GroupName
         self.table_with_caption_first_title_is_centered(ResultTool.sort(PIH.RESULT.MARK.free_list(show_guest_marks), sort_function), "Свободные карты доступа:", use_index)
 
     def guest_marks(self, use_index: bool = False) -> None:
-        mark_list_result: Result[List[Mark]] = PIH.RESULT.MARK.free_list(True)
+        mark_list_result: Result[list[Mark]] = PIH.RESULT.MARK.free_list(True)
         mark_list_result.fields.visible(
             FIELD_NAME_COLLECTION.GROUP_NAME, False)
         def filter_function(item: Mark) -> bool:
             return EnumTool.get(MarkType, item.type) == MarkType.GUEST
         ResultTool.filter(mark_list_result, filter_function)
         self.table_with_caption_first_title_is_centered(
             mark_list_result, "Гостевые карты доступа:", use_index)
@@ -913,31 +962,31 @@
 
     def free_marks_by_group_for_result(self, group: MarkGroup, result: Result, use_index: bool) -> None:
         group_name: str = group.GroupName
         self.table_with_caption_last_title_is_centered(
             result, f"Свободные карты доступа для группы доступа '{group_name}':", use_index)
 
     def temporary_marks(self, use_index: bool = False,) -> None:
-        def modify_table(table: PrettyTable, caption_list: List[str]):
+        def modify_table(table: PrettyTable, caption_list: list[str]):
             table.align[caption_list[0]] = "c"
             table.align[caption_list[1]] = "c"
         self.table_with_caption(
             PIH.RESULT.MARK.temporary_list(), "Список временных карт:", use_index, modify_table)
 
     def containers_for_result(self, result: Result, use_index: bool = False) -> None:
         self.table_with_caption(result, "Подразделение:", use_index)
 
     def table_with_caption_first_title_is_centered(self, result: Result, caption: str, use_index: bool = False, label_function: Callable = None) -> None:
-        def modify_table(table: PrettyTable, caption_list: List[str]):
+        def modify_table(table: PrettyTable, caption_list: list[str]):
             table.align[caption_list[int(use_index)]] = "c"
         self.table_with_caption(
             result, caption, use_index, modify_table, label_function)
 
     def table_with_caption_last_title_is_centered(self, result: Result, caption: str, use_index: bool = False, label_function: Callable = None) -> None:
-        def modify_table(table: PrettyTable, caption_list: List[str]):
+        def modify_table(table: PrettyTable, caption_list: list[str]):
             table.align[caption_list[-1]] = "c"
         self.table_with_caption(
             result, caption, use_index, modify_table, label_function)
 
     def table_with_caption(self, result: Any, caption: str = None, use_index: bool = False, modify_table_function: Callable = None, label_function: Callable = None) -> None:
         if caption is not None:
             self.cyan(caption)
@@ -950,28 +999,28 @@
         else:
             if not isinstance(data, list):
                 data = [data]
             if len(data) == 1:
                 use_index = False
             if use_index:
                 field_list.list.insert(0, FIELD_COLLECTION.INDEX)
-            caption_list: List = field_list.get_caption_list()
-            def create_table(caption_list: List[str]) -> PrettyTable:
+            caption_list: list = field_list.get_caption_list()
+            def create_table(caption_list: list[str]) -> PrettyTable:
                 from prettytable.colortable import ColorTable, Themes
                 table: ColorTable = ColorTable(
                     caption_list, theme=Themes.OCEAN)
                 table.align = "l"
                 if use_index:
                     table.align[caption_list[0]] = "c"
                 return table
             table: PrettyTable = create_table(caption_list)
             if modify_table_function is not None:
                 modify_table_function(table, caption_list)
             for index, item in enumerate(data):
-                row_data: List = []
+                row_data: list = []
                 for field_item_obj in field_list.get_list():
                     field_item: FieldItem = field_item_obj
                     if field_item.visible:
                         if field_item.name == FIELD_COLLECTION.INDEX.name:
                             row_data.append(str(index + 1))
                         elif not isinstance(item, dict):
                             if label_function is not None:
@@ -1053,31 +1102,31 @@
                     telephone_number = telehone_number_after_fix
                     self.output.value("Телефон отформатирован", telephone_number)
             if check or PIH.CHECK.telephone_number(telephone_number):
                 return telephone_number
             else:
                 self.output.error("Неверный формат номера телефона!")
 
-    def email(self) -> str:
+    def email(self, title: str | None = None) -> str:
         email: str = None
         while True:
-            email = self.input("Электронная почта")
+            email = self.input(title or "Адресс электронная почта")
             if PIH.CHECK.email(email):
                 return email
             else:
-                self.output.error("Неверный формат электронной почты!")
+                self.output.error("Неверный формат адресса электронной почты!")
 
-    def card_registry_folder(self) -> str:
+    def polibase_person_card_registry_folder(self) -> str:
         value: str = None
         while True:
-            value = self.input("Введите название папки с картами пациентами")
+            value = self.input("Введите название папки с картами пациентов")
             if PIH.CHECK.POLIBASE.person_card_registry_folder_name(value):
-                return value
+                return PIH.DATA.FORMAT.polibase_person_card_registry_folder(value)
             else:
-                self.output.error("Неверный формат названия папки с картами пициентов!")
+                self.output.error("Неверный формат названия папки с картами пациентов!")
 
     def message(self, caption: str = None, prefix: str = None) -> str:
         caption = caption or "Введите сообщение"
         self.output.input(caption)
         return (prefix or "") + self.input(prefix, False)
 
     def description(self) -> str:
@@ -1092,47 +1141,47 @@
                 if check_on_exists and PIH.CHECK.USER.exists_by_login(login):
                     self.output.error("Логин занят!")
                 else:
                     return login
             else:
                 self.output.error("Неверный формат логина!")
 
-    def indexed_list(self, caption: str, name_list: List[Any], caption_list: List[str], by_index: bool = False) -> str:
+    def indexed_list(self, caption: str, name_list: list[Any], caption_list: list[str], by_index: bool = False) -> str:
         return self.item_by_index(caption, name_list, lambda item, index: caption_list[index if by_index else item])
 
     def indexed_field_list(self, caption: str, list: FieldItemList) -> str:
         name_list = list.get_name_list()
         return self.item_by_index(caption, name_list, lambda item, _: list.get_item_by_name(item).caption)
 
-    def index(self, caption: str, data: List, label_function: Callable[[Any, int], str] = None, use_zero_index: bool = False) -> int:
+    def index(self, caption: str, data: list, label_function: Callable[[Any, int], str] = None, use_zero_index: bool = False) -> int:
         selected_index: int = -1
         length: int = len(data)
         has_error: bool = False
         while True:
             min_value: int = 1 - int(use_zero_index)
             max_value: int = length - int(use_zero_index)
             if not has_error and label_function is not None and length > 1:
                 for index, item in enumerate(data):
                     self.output.index(
                             index + 1 - int(use_zero_index) if length > 1 else None, label_function(item, index), max_value)
             if length == 1:
                 return 0
-            selected_index = self.input(
-                caption + f" (от {min_value} до {max_value})")
-            if selected_index == "":
+            selected_index = PIH.DATA.EXTRACT.decimal(self.input(
+                caption + f" (от {min_value} до {max_value})"))
+            if DataTool.is_empty(selected_index):
                 selected_index = min_value
             try:
                 selected_index = int(selected_index) - min_value
                 if selected_index >= 0 and selected_index < length:
                     return selected_index
             except ValueError:
                 has_error = True
                 continue
 
-    def item_by_index(self, caption: str, data: List[Any], label_function: Callable[[Any, int], str] = None, use_zero_index: bool = False) -> Any:
+    def item_by_index(self, caption: str, data: list[Any], label_function: Callable[[Any, int], str] = None, use_zero_index: bool = False) -> Any:
         return data[self.index(caption, data, label_function, use_zero_index)]
 
     def tab_number(self, check: bool = True) -> str:
         tab_number: str = None
         while True:
             tab_number = self.input("Введите номер карты доступа")
             if check:
@@ -1180,15 +1229,15 @@
                     value = value.strip()
                     if PIH.CHECK.name(value):
                         return PIH.DATA.FORMAT.name(value)
                     else:
                         pass
             return FullName(full_name_part("Введите фамилию"), full_name_part("Введите имя"), full_name_part("Введите отчество"))
 
-    def yes_no(self, text: str = " ", enter_for_yes: bool = False, yes_label: str = None, no_label: str = None) -> bool:
+    def yes_no(self, text: str = " ", enter_for_yes: bool = False, yes_label: str = None, no_label: str = None, yes_checker: Callable[[str], bool] = None) -> bool:
         text = self.output.blue_str(self.output.text_color(Fore.WHITE, text))
         self.output.write_line(f"{text}? \n{self.output.green_str(self.output.text_black('Да (1 или Ввод)'))} / {self.output.red_str(self.output.text_black('Нет (Остальное)'), '')}" if enter_for_yes else
                                f"{text}? \n{self.output.red_str('Да (1)')} / {self.output.green_str(self.output.text_black('Нет (Остальное или Ввод)'), '')}")
         answer: str = self.input()
         answer = answer.lower()
         self.answer = answer
         return answer == "y" or answer == "yes" or answer == "1" or (answer == "" and enter_for_yes)
@@ -1199,31 +1248,30 @@
             head_string = f"Здравствуйте, {FullNameTool.to_given_name(user.name)}, "
             self.output.green(head_string)
             message = self.input("Введите сообщениеt: ")
             return head_string + message
         else:
             pass
 
-    def polibase_person_any(self) -> str:
-        return self.input(
-            "Введите персональный номер или часть имени пациента")
+    def polibase_person_any(self, title: str | None = None) -> str:
+        return self.input(title or "Введите персональный номер или часть имени пациента")
 
 
 class MarkInput(MarkInputBase):
 
     def __init__(self, input: Input = None):
         self.parent = input
 
     def free(self, group: MarkGroup = None) -> Mark:
-        result: Result[List[Mark]] = None
+        result: Result[list[Mark]] = None
         while True:
             if group is None:
                 if self.parent.yes_no("Выбрать группы доступа для карты доступа, введя имени пользователя из этой группы"):
                     result = PIH.RESULT.MARK.by_name(self.parent.name())
-                    mark_list: List[Mark] = result.data
+                    mark_list: list[Mark] = result.data
                     length = len(mark_list)
                     if length > 0:
                         if length > 1:
                             self.parent.output.table_with_caption_first_title_is_centered(
                                 result, "Найденные пользователи:", True)
                         group = self.parent.item_by_index(
                             "Выберите группу доступа", mark_list)
@@ -1255,32 +1303,32 @@
                         "Выберите карту доступа введя индекс", data)
                 else:
                     self.parent.output.error(
                         f"Нет свободных карт для группы доступа '{group.GroupName}'!")
                     return self.free()
 
     def person_division(self) -> MarkDivision:
-        division_list: List[MarkDivision] = PIH.RESULT.MARK.person_divisions().data
+        division_list: list[MarkDivision] = PIH.RESULT.MARK.person_divisions().data
         division_list.insert(0, MarkDivision(0, "Без подразделения"))
         return self.parent.item_by_index("Выберите подразделение для персоны, которой принадлежит карта доступа", division_list, lambda item, _: item.name )
 
     def by_name(self) -> Mark:
         self.parent.output.head2("Введите имя персоны")
-        result: Result[List[Mark]] = None
+        result: Result[list[Mark]] = None
         while result is None:
             try:
                 result = PIH.RESULT.MARK.by_name(
                     self.parent.name())
             except NotFound as error:
                 self.parent.output.error(error.get_details())
         self.parent.output.mark.result(result, "Карты доступа", True)
         return self.parent.item_by_index("Выберите карточку, введя индекс", result.data)
 
     def by_any(self, value: str = None) -> Mark:
-        result: Result[List[Mark]] = None
+        result: Result[list[Mark]] = None
         while result is None:
             try:
                 result = PIH.RESULT.MARK.by_any(value or self.any())
             except NotFound as error:
                 self.parent.output.error(error.get_details())
         self.parent.output.mark.result(result, "Карты доступа", True)
         return self.parent.item_by_index("Выберите карточку, введя индекс", result.data)
@@ -1292,30 +1340,30 @@
 
 class UserInput(UserInputBase):
 
     def __init__(self, input: Input = None):
         self.parent = input
 
     def container(self) -> UserContainer:
-        result: Result[List[UserContainer]] = PIH.RESULT.USER.containers()
+        result: Result[list[UserContainer]] = PIH.RESULT.USER.containers()
         self.parent.output.containers_for_result(result, True)
         return self.parent.item_by_index("Выберите контейнер пользователя, введя индекс", result.data)
 
     def by_name(self) -> User:
-        result: Result[List[User]] = PIH.RESULT.USER.by_name(
+        result: Result[list[User]] = PIH.RESULT.USER.by_name(
             self.parent.name())
         result.fields = FIELD_COLLECTION.AD.USER_NAME
         self.parent.output.table_with_caption(
             result, "Список пользователей", True)
         return self.parent.item_by_index("Выберите пользователя, введя индекс", result.data)
 
     def title_any(self, title: str = None) -> str:
         return self.parent.input(title or "Введите логин, часть имени или другой поисковый запрос")
 
-    def by_any(self, value: str = None, active: bool = None, title: str = None, use_all: bool = False) -> List[User]:
+    def by_any(self, value: str = None, active: bool = None, title: str = None, use_all: bool = False) -> list[User]:
         result: Result[list[User]] = PIH.RESULT.USER.by_any(value or self.title_any(title), active)
         label_function: Callable[[Any, int], str] = (lambda item, _: "Все" if item is None else item.name) if len(
             result.data) > 1 else None
         if use_all and len(result.data) > 1:
             result.data.append(None)
         result_data: User = self.parent.item_by_index("Выберите пользователя, введя индекс", result.data, label_function)
         return result.data if result_data is None else [result_data]
@@ -1324,43 +1372,43 @@
         try:
             return self.by_any(value, active, title)
         except NotFound:
             return None
 
 
     def template(self) -> dict:
-        result: Result[List[User]] = PIH.RESULT.USER.template_list()
+        result: Result[list[User]] = PIH.RESULT.USER.template_list()
         self.parent.output.template_users_for_result(result, True)
         return self.parent.item_by_index("Выберите шаблон пользователя, введя индекс", result.data)
 
     def search_attribute(self) -> str:
         return self.parent.indexed_field_list("Выберите по какому критерию искать, введя индекс",
                                              FIELD_COLLECTION.AD.SEARCH_ATTRIBUTE)
 
     def search_value(self, search_attribute: str) -> str:
         field_item = FIELD_COLLECTION.AD.SEARCH_ATTRIBUTE.get_item_by_name(
             search_attribute)
         return self.parent.input(f"Введите {field_item.caption.lower()}")
 
     def generate_password(self, once: bool = False, settings: PasswordSettings = PASSWORD.SETTINGS.DEFAULT) -> str:
-        def generate_password_interanal(settings: PasswordSettings = None) -> str:
+        def internal_generate_password(settings: PasswordSettings = None) -> str:
             return PasswordTools.generate_random_password(settings.length, settings.special_characters,
                                                           settings.order_list, settings.special_characters_count,
                                                           settings.alphabets_lowercase_count, settings.alphabets_uppercase_count,
                                                           settings.digits_count, settings.shuffled)
         while True:
-            password = generate_password_interanal(settings)
-            if once or self.parent.yes_no(f"Использовать пароль {password} ", True):
+            password = internal_generate_password(settings)
+            if once or self.parent.yes_no(f"Использовать пароль {password}", True):
                 return password
             else:
                 pass
 
     def generate_login(self, full_name: FullName, ask_for_remove_inactive_user_if_login_is_exists: bool = True, ask_for_use: bool = True) -> str:
-        login_list: List[str] = []
-        inactive_user_list: List[User] = []
+        login_list: list[str] = []
+        inactive_user_list: list[User] = []
         login_is_exists: bool = False
 
         def show_user_which_login_is_exists_and_return_user_if_it_inactive(login_string: str) -> User:
             user: User = PIH.RESULT.USER.by_login(login_string).data
             is_active: bool = PIH.CHECK.USER.active(user)
             self.parent.output.error(
                 f"Логин '{login_string}' занят {'активным' if is_active else 'неактивным'} пользователем: {user.name}")
@@ -1389,40 +1437,38 @@
                         self.parent.output.error("Ошибка")
                 else:
                     need_enter_login = True
             else:
                 need_enter_login = True
             return need_enter_login, login_string
         if PIH.CHECK.USER.exists_by_login(login_string):
-            user: User = show_user_which_login_is_exists_and_return_user_if_it_inactive(
-                login_string)
+            user: User = show_user_which_login_is_exists_and_return_user_if_it_inactive(login_string)
             if user is not None:
                 inactive_user_list.append(user)
-            login_alt: FullName = NamePolicy.convert_to_alternative_login(
-                login)
+            login_alt: FullName = NamePolicy.convert_to_alternative_login(login)
             login_string = FullNameTool.to_string(login_alt, "")
             login_is_exists = login_string in login_list
             if not login_is_exists:
                 login_list.append(login_string)
             if login_is_exists or PIH.CHECK.USER.exists_by_login(login_string):
                 if not login_is_exists:
                     user = show_user_which_login_is_exists_and_return_user_if_it_inactive(
                         login_string)
                     if user is not None:
                         inactive_user_list.append(user)
-                login_reversed: FullName = NamePolicy.convert_to_reverse_login(
-                    login)
+                login_reversed: FullName = NamePolicy.convert_to_reverse_login(login)
                 login_is_exists = login_string in login_list
                 login_string = FullNameTool.to_string(login_reversed, "")
                 if not login_is_exists:
                     login_list.append(login_string)
                 if login_is_exists or PIH.CHECK.USER.exists_by_login(login_string):
+                    login_last: FullName = NamePolicy.convert_to_last_login(login)
+                    login_string = FullNameTool.to_string(login_last, "")
                     if not login_is_exists:
-                        user = show_user_which_login_is_exists_and_return_user_if_it_inactive(
-                            login_string)
+                        user = show_user_which_login_is_exists_and_return_user_if_it_inactive(login_string)
                         if user is not None:
                             inactive_user_list.append(user)
                     if ask_for_remove_inactive_user_if_login_is_exists and len(inactive_user_list) > 0:
                         need_enter_login, login_string = remove_inactive_user_action()
                     if need_enter_login:
                         while True:
                             login_string = self.parent.login()
@@ -1504,21 +1550,26 @@
             NamePolicy.get_first_letter(full_name.middle_name))
 
     @staticmethod
     def convert_to_alternative_login(login_list: FullName) -> FullName:
         return FullName(login_list.first_name, login_list.middle_name, login_list.last_name)
 
     @staticmethod
+    def convert_to_last_login(login_list: FullName) -> FullName:
+        return FullName(login_list.first_name, login_list.last_name, login_list.middle_name)
+
+    @staticmethod
     def convert_to_reverse_login(login_list: FullName) -> FullName:
         return FullName(login_list.middle_name, login_list.first_name, login_list.last_name)
 
 
 class PIH:
 
     NAME: str = "pih"
+    NAME_ALT: str = "пих"
 
     def __init__(self, input: InputBase = None, output: OutputBase = None, session: SessionBase = None): 
         if output is None:
             output = Output(UserOutput(), MarkOutput())
             PIH.output: Output = output
         else:
             self.output: Output = output
@@ -1529,29 +1580,48 @@
         else:
             self.input: Input = input
         if session is None: 
             PIH.session: Session = Session(input, output)
         else:
             self.session: Session = session
         
+    class MOBILE_HELPER:
+
+        ANSWER: dict[str, list[str]] = defaultdict(list)
+
+        @staticmethod
+        def create_output(recipient: str) -> Output:
+            return PIH.MESSAGE.WHATSAPP.create_output(recipient)
+
+        @staticmethod
+        def waiting_for_input_from(recipient: str, handler: Callable[[str, Callable[[None], None]], None] | None = None) -> str | None:
+            def internal_handler(message: str, close_handler: Callable[[None], None]) -> None:
+                PIH.MOBILE_HELPER.ANSWER[recipient].append(message)
+                if DataTool.is_empty(handler):
+                    close_handler()
+                else:
+                    handler(message, close_handler)  
+            PIH.EVENT.waiting_for_mobile_helper_message_input(
+                recipient, internal_handler)
+            return PIH.MOBILE_HELPER.ANSWER[recipient][-1] 
 
     class VERSION:
 
         @staticmethod
         def local() -> str:
-            return "1.421"
+            return "1.43"
 
         @staticmethod
         def need_update() -> bool:
             return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
 
         @staticmethod
         def remote() -> str:
             try:
-                req = requests.get(CONST.PYPI_URL)
+                req = requests.get(URLS.PYPI)
                 version = parse("0")
                 if req.status_code == requests.codes.ok:
                     data = json.loads(req.text.encode(req.encoding))
                     releases = data.get("releases", [])
                     for release in releases:
                         ver = parse(release)
                         if not ver.is_prerelease:
@@ -1562,39 +1632,39 @@
 
     class ERROR:
 
         notify_about_error: bool = True
 
         @staticmethod
         def create_error_header(details: str) -> str:
-            return f"\nВерсия: {PIH.VERSION.local()}/{PIH.VERSION.remote()}\nПользователь: {PIH.OS.get_login()}\nКомпьютер: {PIH.OS.get_host()}\n{details}"
+            return f"\nВерсия: {PIH.VERSION.local()}/{PIH.VERSION.remote()}\nПользователь: {PIH.OS.get_login()}\nКомпьютер: {PIH.OS.host()}\n{details}"
 
         @staticmethod
-        def rpc_error_handler(details: str, code: Tuple, role: ServiceRoles, command: ServiceCommands) -> None:
+        def rpc_error_handler(details: str, code: Tuple, service_role_description: ServiceRoles, command: ServiceCommands) -> None:
             if isinstance(command, ServiceCommands):
                 if code == StatusCode.UNAVAILABLE:
                     PIH.output.error(f"Error: {details}")
                     return
                 elif code == StatusCode.DEADLINE_EXCEEDED or details.lower().find("stream removed") != -1:
                     return
                 else:
                     if PIH.ERROR.notify_about_error:
-                        PIH.LOG.from_debug_bot(
+                        PIH.LOG.debug(
                             PIH.ERROR.create_error_header(details), LogLevels.ERROR)
             raise Error(details, code) from None
 
         @staticmethod
         def global_except_hook(exctype, value, __traceback__):
-            details_list: List[str] = []
+            details_list: list[str] = []
             for item in value.args:
                 if isinstance(item, str):
                     details_list.append(item)
             details: str = "\n".join(traceback.format_exception(value))
             if PIH.ERROR.notify_about_error:
-                PIH.LOG.from_debug_bot(
+                PIH.LOG.debug(
                     PIH.ERROR.create_error_header(details), LogLevels.ERROR)
             sys.__excepthook__(exctype, value, traceback)
 
         sys.excepthook = global_except_hook
 
         class POLIBASE:
 
@@ -1616,40 +1686,39 @@
                     start = "Неактивный пользователь"
                 return NotFound(f"{start} с {title} '{value}' не найден", value)
 
     class UPDATER:
 
         @staticmethod
         def update_for_service(service_role: ServiceRoles, pih_update: bool = True, modules_update: bool = True, show_output: bool = False) -> bool:
-            service_role_value: ServiceRoleDescription = service_role.value
+            service_role_description: ServiceRoleDescription = service_role.value
             returncode: int = 0
             if pih_update:
-                remote_executor_command_list: List[str] = PIH.PSTOOLS.create_remote_process_executor_for_service_role(
-                    service_role, True)
-                command_list: List[str] = remote_executor_command_list + \
+                remote_executor_command_list: list[str] = PIH.PSTOOLS.create_remote_process_executor_for_service(service_role_description, True)
+                command_list: list[str] = remote_executor_command_list + \
                     PIH.UPDATER.get_module_updater_command_list(PIH.NAME, None)
                 process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(
                     command_list, show_output)
                 returncode = process_result.returncode
             result: bool = returncode == 0
             if modules_update and result:
-                installed_module_list: List[str] = {
+                installed_module_list: list[str] = {
                     pkg.key.lower() for pkg in pkg_resources.working_set}
-                for module_name in [item.lower() for item in service_role_value.modules]:
+                for module_name in [item.lower() for item in service_role_description.modules]:
                     if module_name not in installed_module_list:
                         result = result and PIH.UPDATER.install_module(
                             module_name, show_output=show_output)
                         if result:
                             pkg_resources.working_set.add_entry(module_name)
                         else:
                             break
             return result
 
         @staticmethod
-        def get_module_updater_command_list(module_name: str, version: str = None) -> List[str]:
+        def get_module_updater_command_list(module_name: str, version: str = None) -> list[str]:
             return ["-m", CONST.PYTHON.PYPI, "install"] + ([f"{module_name}=={version}"] if version is not None else [module_name, "-U"])
 
         @staticmethod
         def update_localy(version: str = None, show_output: bool = False) -> bool:
             return PIH.UPDATER.install_module(PIH.NAME, version, show_output)
 
         @staticmethod
@@ -1660,17 +1729,17 @@
             process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(
                 command_list, show_output)
             returncode = process_result.returncode
             return returncode == 0
 
         @staticmethod
         def update_remote(host: str, show_output: bool = False) -> bool:
-            remote_executor_command_list: List[str] = PIH.PSTOOLS.create_command_list_for_psexec_command(
+            remote_executor_command_list: list[str] = PIH.PSTOOLS.create_command_list_for_psexec_command(
                 host)
-            command_list: List[str] = remote_executor_command_list + \
+            command_list: list[str] = remote_executor_command_list + \
                 PIH.UPDATER.get_module_updater_command_list()
             process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(
                 command_list, show_output)
             returncode = process_result.returncode
             return returncode == 0
 
         @staticmethod
@@ -1690,14 +1759,22 @@
                     start_handler()
             Thread(target=internal_update_action, args=(
                 need_update, start_handler, update_start_handler, update_complete_handler,)).start()
 
     class SETTINGS:
 
         @staticmethod
+        def to_datetime(value: SETTINGS) -> datetime:
+            return PIH.DATA.CONVERT.settings_to_datetime(value)
+        
+        @staticmethod
+        def to_datetime_list(value: SETTINGS) -> list[datetime]:
+            return PIH.DATA.CONVERT.settings_to_datetime_list(value)
+
+        @staticmethod
         def set(settings_item: SETTINGS, value: Any) -> bool:
             return PIH.ACTION.SETTINGS.set(settings_item, value)
 
         @staticmethod
         def set_default(settings_item: SETTINGS) -> bool:
             return PIH.ACTION.SETTINGS.set_default(settings_item)
 
@@ -1711,52 +1788,59 @@
                 if setting_item.value.auto_init:
                     PIH.SETTINGS.set_default(setting_item)
 
         class WORKSTATION:
 
             @staticmethod
             def shutdown_time() -> datetime:
-                return DateTimeTool.from_string(PIH.SETTINGS.get(SETTINGS.WORKSTATION_SHUTDOWN_TIME), CONST.SECONDLESS_TIME_FORMAT)
+                return PIH.DATA.CONVERT.settings_to_datetime(SETTINGS.WORKSTATION_SHUTDOWN_TIME)
             
             @staticmethod
             def reboot_time() -> datetime:
-                return DateTimeTool.from_string(PIH.SETTINGS.get(SETTINGS.WORKSTATION_REBOOT_TIME), CONST.SECONDLESS_TIME_FORMAT)
+                return PIH.DATA.CONVERT.settings_to_datetime(SETTINGS.WORKSTATION_REBOOT_TIME)
 
         class USER:
 
             @staticmethod
             def use_cache() -> bool:
-                return True
+                return PIH.SETTINGS.get(SETTINGS.USER_USE_CACHE)
             
-        class RESOURCE_MANAGER:
+        class INDICATION:
+
+            @staticmethod
+            def ct_notification_start_time() -> list[datetime]:
+                return PIH.DATA.CONVERT.settings_to_datetime(SETTINGS.INDICATION_CT_NOTIFICATION_START_TIME)
+            
+        class RESOURCE:
     
             @staticmethod
             def site_check_certificate_start_time() -> datetime:
-                return DateTimeTool.from_string(PIH.SETTINGS.get(SETTINGS.RESOURCE_MANAGER_CHECK_SITE_CERTIFICATE_START_TIME), CONST.SECONDLESS_TIME_FORMAT)
+                return PIH.DATA.CONVERT.settings_to_datetime(
+                    SETTINGS.RESOURCE_MANAGER_CHECK_SITE_CERTIFICATE_START_TIME)
             
             @staticmethod
             def site_check_free_spcae_perion_in_minutes() -> int:
                 return PIH.SETTINGS.get(SETTINGS.RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES)
 
 
         class POLIBASE:
 
             @staticmethod
-            def test_telephone_number(sender: Any) -> str:
+            def test_recipient(sender: Any) -> str | None:
                 if sender == CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.CALL_CENTRE.value:
                     return PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_VISIT_NOTIFICATION_TEST_TELEPHONE_NUMBER)
                 if sender == CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.MARKETER.value:
                     return PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_REVIEW_NOTIFICATION_TEST_TELEPHONE_NUMBER)
                 return None
             
-            class REVIEW:
+            class REVIEW_NOTIFICATION:
 
                 @staticmethod
                 def start_time() -> datetime:
-                    return DateTimeTool.from_string(PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME), CONST.SECONDLESS_TIME_FORMAT)
+                    return PIH.DATA.CONVERT.settings_to_datetime(SETTINGS.POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME)
 
                 @staticmethod
                 def is_on() -> bool:
                     return PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON)
 
                 @staticmethod
                 def day_delta() -> int:
@@ -1765,81 +1849,154 @@
                 @staticmethod
                 def notification_text(person: PolibasePerson, notification_confirmed: bool) -> str:
                     return str(PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION if notification_confirmed else SETTINGS.POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT)).format(name=FullNameTool.to_given_name(person))
 
             class VISIT:
 
                 @staticmethod
-                def get_offer_telegram_bot_url_text(person_full_name: str) -> str:
+                def offer_telegram_bot_url_text(person_full_name: str) -> str:
                     return str(PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_TEXT)).format(name=FullNameTool.to_given_name(person_full_name)) 
 
     class PSTOOLS:
 
         @staticmethod
+        def ping(address_or_ip: str, host: str, count: int = 1, timeout: int = 100):
+            command_list: list[str] = ["ping", "-4",  address_or_ip, "-n",
+                                       str(count), "-w", str(timeout)]
+            result: CompletedProcess = PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(command_list, host, interactive=True), True, True)
+            out: str = result.stdout
+            return result.returncode == 0 and out.count("(TTL)") < count
+          
+        @staticmethod
         def get_executor_path(executor_name: str) -> str:
             return os.path.join(
                 PATHS.WS.PATH, CONST.PSTOOLS.NAME, executor_name)
 
-        def get_host(value: str) -> str:
+        @staticmethod
+        def as_host(value: str) -> str:
             host_start: str = r"\\"
             return ("" if value.startswith(host_start) else host_start) + value 
 
         @staticmethod
-        def create_command_list_for_command(executor_name: str, command_list: List[str], login: str = None, password: str = None) -> List[str]:
-            login = login or "\\".join([CONST.AD.DOMAIN_NAME, CONST.AD.ADMINISTRATOR])
-            password = password or CONST.AD.ADMINISTRATOR_PASSOWORD
+        def create_command_list_for_command(executor_name: str, command_list: list[str], login: str = None, password: str = None) -> list[str]:
+            login = "\\".join([AD.DOMAIN_NAME, AD.ADMINISTRATOR if DataTool.is_empty(login) else login])
+            password = password or AD.ADMINISTRATOR_PASSOWORD
             return [PIH.PSTOOLS.get_executor_path(executor_name), CONST.PSTOOLS.NO_BANNER, CONST.PSTOOLS.ACCEPTEULA, "-u", login, "-p", password]  + command_list
         
         @staticmethod
-        def create_command_list_for_psexec_command(command_list: List[str], host: str = None, login: str = None, password: str = None, interactive: bool = False, run_from_system_account: bool = False, run_with_elevetion: bool = False) -> List[str]:
-            result_command_list: List[str] = ["-i" if interactive else "-d"]
+        def create_command_list_for_psexec_command(command_list: list[str], host: str = None, login: str = None, password: str = None, interactive: bool = False, run_from_system_account: bool = False, run_with_elevetion: bool = False) -> list[str]:
+            result_command_list: list[str] = ["-i" if interactive else "-d"]
             host_start: str = r"\\"
             if not DataTool.is_empty(host):
                 result_command_list.append(("" if host.startswith(host_start) else host_start) + host)
             if run_from_system_account:
                 result_command_list.append("-s")
             if run_with_elevetion:
                 result_command_list.append("-h")
             return PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_EXECUTOR, result_command_list + command_list, login, password)
 
         @staticmethod
-        def create_command_list_for_pstools_command(command_name: str, command_list: List[str],  login: str = None, password: str = None) -> List[str]:
-            return PIH.PSTOOLS.create_command_list_for_command(command_name, command_list, login, password)
-
-        @staticmethod
-        def create_remote_process_executor_for_service_role(value: ServiceRoles, interactive: bool = False) -> List[str]:
-            service_role_value: ServiceRoleDescription = value.value
-            return PIH.PSTOOLS.create_command_list_for_psexec_command([CONST.PYTHON.EXECUTOR], PIH.SERVICE.get_host(value), service_role_value.login, service_role_value.password, interactive)
+        def create_remote_process_executor_for_service(service_role_or_description: ServiceRoles | ServiceRoleDescription, interactive: bool = False) -> list[str]:
+            service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+            return PIH.PSTOOLS.create_command_list_for_psexec_command([CONST.PYTHON.EXECUTOR], PIH.SERVICE.get_host(service_role_description), service_role_description.login, service_role_description.password, interactive)
 
         @staticmethod
-        def execute_command_list(command_list: List[str], show_output: bool, capture_output: bool = False) -> CompletedProcess:
-            subprocess.check_output
+        def execute_command_list(command_list: list[str], show_output: bool, capture_output: bool = False) -> CompletedProcess:
             if show_output:
                 if capture_output:
                     process_result = subprocess.run(
                         command_list, capture_output=True, text=True)
                 else:
                     process_result = subprocess.run(
                         command_list, text=True)
             else:
                 process_result = subprocess.run(
                     command_list, stdout=DEVNULL, stderr=STDOUT, text=True)
             return process_result
        
         @staticmethod
-        def kill_process(name: str, host: str, show_output: bool = False) -> bool:
-           return PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_KILL_EXECUTOR, ["-t", name, PIH.PSTOOLS.get_host(host)]), show_output).returncode == 0
+        def kill_process(name_or_pid: str | int, host: str, show_output: bool = False) -> bool:
+           return PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_KILL_EXECUTOR, ["-t", str(name_or_pid), PIH.PSTOOLS.as_host(host)]), show_output).returncode == 0
+
+        @staticmethod
+        def kill_process_via_windows(name_or_pid: str | int, host: str, show_output: bool = False) -> bool:
+           is_string : bool = isinstance(name_or_pid, str)
+           return PIH.PSTOOLS.execute_command_list(["taskkill", "/S", PIH.PSTOOLS.as_host(host), "/F", "/IM" if is_string else "/PID", PIH.PATH.add_extension(name_or_pid, FILE.EXTENSION.EXE) if is_string else str(name_or_pid)], show_output).returncode == 0
+
+        @staticmethod
+        def reboot(host: str, show_output: bool = False) -> bool:
+            return PIH.PSTOOLS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+                ["shutdown", "/r", "/t", "0"], host), show_output).returncode == 0
 
+        @staticmethod
+        def shutdown(host: str, show_output: bool = False) -> bool:
+            return PIH.PSTOOLS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+                ["shutdown", "/s", "/t", "0"], host), show_output).returncode == 0
+        
+    class EVENT:
+
+        @staticmethod
+        def on_log_command(handler: Callable[[ParameterList, ServiceListener], None]) -> None:
+            ServiceListener().listen_for([ServiceCommands.send_log_command], lambda _, parameter_list, service_listener: handler(parameter_list, service_listener))
+
+        @staticmethod
+        def wait_server_start(handler_or_server_name: Callable[[str, Callable[[None], None]], None] | str) -> None:
+            def internal_handler(parameter_list: ParameterList, listener: ServiceListener) -> None:
+                log_command, parameters = PIH.DATA.EXTRACT.SERVICE_PARAMETER_LIST.log_command_parameters(parameter_list)
+                if log_command == LogCommands.SERVER_WAS_STARTED:
+                    server_name: str = parameters[0]
+                    if callable(handler_or_server_name):
+                        handler_or_server_name(server_name, listener.close)
+                    else:
+                        if handler_or_server_name.startswith(server_name):
+                            listener.close()
+            PIH.EVENT.on_log_command(internal_handler)
+
+        @staticmethod
+        def wait_robocopy_job_complete(handler_or_robocopy_job_name: Callable[[ParameterList, ServiceListener], None] | str) -> None:
+            def internal_handler(parameter_list: ParameterList, listener: ServiceListener) -> None:
+                log_command, parameters = PIH.DATA.EXTRACT.SERVICE_PARAMETER_LIST.log_command_parameters(parameter_list)
+                if log_command ==  A.CT_LC.BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_COMPLETED:
+                    robocopy_job_status: str = parameters[0]
+                    if callable(handler_or_robocopy_job_name):
+                        handler_or_robocopy_job_name(
+                            robocopy_job_status, listener.close)
+                    else:
+                        if robocopy_job_status.startswith(handler_or_robocopy_job_name):
+                            listener.close()
+            PIH.EVENT.on_log_command(internal_handler)
+
+        @staticmethod
+        def waiting_for_mobile_helper_message_input(recipient: str, handler: Callable[[str, Callable[[None], None]], None]) -> None:
+            def internal_handler(parameter_list: ParameterList, listener: ServiceListener) -> None:
+                message: WhatsAppMessage = PIH.DATA.EXTRACT.SERVICE_PARAMETER_LIST.whatsapp_message(parameter_list)
+                if not DataTool.is_empty(message) and PIH.DATA.FORMAT.telephone_number(message.sender) == PIH.DATA.FORMAT.telephone_number(recipient):
+                    handler(message.message, listener.close)
+            PIH.EVENT.on_log_command(internal_handler)
+
+            
     class SERVICE:
 
-        command_map: dict = None
+        command_map: dict[str, ServiceRoleDescription] = None
 
         class ADMIN:
 
             @staticmethod
+            def call(service_command: ServiceCommands, parameters: Any) -> str:
+                return RPC.call(service_command, parameters)
+
+            @staticmethod
+            def subscribe_on(service_command: ServiceCommands, type: int = SubscribtionTypes.AFTER, name: str = None) -> bool:
+                return RPC.Service.service.subscribe_on(service_command, type, name)
+
+            @staticmethod
+            def unsubscribe(service_command: ServiceCommands, type: int) -> bool:
+                return RPC.Service.service.unsubscribe(service_command, type)
+
+            @staticmethod
             def create_developer_service_role_description(port: int = None) -> ServiceRoleDescription:
                 if port is None or port == ServiceRoles.DEVELOPER.value.port:
                     return ServiceRoles.DEVELOPER.value
                 return ServiceRoleDescription(f"Developer{port}", host=CONST.HOST.DEVELOPER.NAME, port=CONST.RPC.PORT(port))
 
             @staticmethod
             def develope(service_role: ServiceRoles, port: int = None) -> None:
@@ -1847,133 +2004,169 @@
                 service_role_description: ServiceRoleDescription = service_role.value
                 service_role_description.auto_restart = False
                 service_role_description.host = developer_service_role_description.host
                 service_role_description.port = developer_service_role_description.port
 
             @staticmethod
             def isolate(service_role: ServiceRoles) -> None:
-                service_role_value: ServiceRoleDescription = service_role.value
-                service_role_value.isolated = True
+                service_role_description: ServiceRoleDescription = service_role.value
+                service_role_description.isolated = True
 
             @staticmethod
-            def start(service_role: ServiceRoles, check_if_started: bool = True, show_output: bool = False) -> bool:
+            def start(service_role_or_description: ServiceRoles | ServiceRoleDescription, check_if_started: bool = True, show_output: bool = False) -> bool:
+                service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
                 if check_if_started:
-                    if PIH.SERVICE.check_accessibility(service_role):
+                    if PIH.SERVICE.check_accessibility(service_role_description):
                         return None
-                service_role_value: ServiceRoleDescription = service_role.value
-                remote_executor_command_list: List[str] = PIH.PSTOOLS.create_remote_process_executor_for_service_role(service_role)
+                remote_executor_command_list: list[str] = PIH.PSTOOLS.create_remote_process_executor_for_service(service_role_description)
                 service_file_path: str = None
-                if service_role_value.service_path is None:
+                if service_role_description.service_path is None:
                     service_file_path = os.path.join(
-                        CONST.FACADE.PATH, f"{service_role_value.name}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", f"{CONST.SERVICE.NAME}.{FILE.EXTENSION.PYTHON}")
+                        CONST.FACADE.PATH, f"{service_role_description.name}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
                 else:
                     service_file_path = os.path.join(
-                        service_role_value.service_path, f"{CONST.SERVICE.NAME}.{FILE.EXTENSION.PYTHON}")
+                        service_role_description.service_path, PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
                 remote_executor_command_list.append(service_file_path)
                 #debug = False
                 remote_executor_command_list.append("False")
                 process_result = PIH.PSTOOLS.execute_command_list(
                     remote_executor_command_list, show_output)
                 returncode = process_result.returncode
                 if returncode == 2:
                     return False
-                service_role_value.pid = returncode
+                service_role_description.pid = returncode
                 return True
 
             @staticmethod
-            def stop(role: ServiceRoles, show_output: bool = False) -> bool:
-                if PIH.SERVICE.check_accessibility(role):
-                    service_role_value: ServiceRoleDescription = role.value
-                    host: str = "\\\\" + PIH.SERVICE.get_host(role)
-                    ps_kill_executor_path: str = PIH.PSTOOLS.get_executor_path(CONST.PSTOOLS.PS_KILL_EXECUTOR)
-                    process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(
-                        [ps_kill_executor_path, host, str(service_role_value.pid)], show_output)
-                    returncode = process_result.returncode
-                    result: bool = returncode == 0
-                    if result:
-                        service_role_value.pid = -1
-                    return result
+            def kill_via_pstools(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> bool | None:
+                service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+                if PIH.SERVICE.check_accessibility(service_role_description):
+                    return PIH.PSTOOLS.kill_process(service_role_description.pid, PIH.PSTOOLS.as_host(PIH.SERVICE.get_host(service_role_description)))
                 return None
-
-
+            
             @staticmethod
-            def publish(service_role: ServiceRoles) -> None:
-                service_role_value: ServiceRoleDescription = service_role.value
-                PIH.ACTION.DATA_STORAGE.value(service_role_value)
+            def kill(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> bool: # | None:
+                service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+                #if PIH.SERVICE.check_accessibility(service_role_description):
+                return PIH.PSTOOLS.kill_process_via_windows(service_role_description.pid, PIH.PSTOOLS.as_host(PIH.SERVICE.get_host(service_role_description)))
+                #return None
+            
+            @staticmethod
+            def serve(service_role_or_description: ServiceRoles | ServiceRoleDescription, call_handler: Callable[[str, ParameterList, Any], Any], isolate: bool = False, service_started_handler: Callable[[None], None] = None, depends_on_list: list[ServiceRoles | ServiceRoleDescription] = [], max_workers=None, stop_before: bool = False) -> RPC.Service:
+                if stop_before:
+                    if PIH.SERVICE.check_accessibility(service_role_or_description):
+                        PIH.SERVICE.ADMIN.stop(service_role_or_description)
+                service: RPC.Service = RPC.Service()
+                service.serve(service_role_or_description, call_handler, isolate, service_started_handler, depends_on_list, max_workers)
 
             @staticmethod
-            def receive(service_role: ServiceRoles) -> ServiceRoleDescription:
-                service_role_value: ServiceRoleDescription = service_role.value
-                return PIH.RESULT.DATA_STORAGE.value(service_role_value.name, ServiceRoleDescription)
+            def stop(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> None:
+                service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(
+                            service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+                if PIH.SERVICE.check_accessibility(service_role_description):
+                    RPC.stop(service_role_description)  
+                    PIH.SERVICE.ADMIN.kill(service_role_description)   
+            
+            @staticmethod
+            def publish(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> bool:
+                role_descrption: ServiceRoleDescription = service_role_or_description if isinstance(
+                    service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+                return PIH.ACTION.DATA_STORAGE.value(role_descrption)
+            
+            @staticmethod
+            def receive(name: str) -> ServiceRoleDescription:
+                return PIH.RESULT.DATA_STORAGE.value(name, ServiceRoleDescription)
 
         @staticmethod
-        def check_accessibility(role: ServiceRoles) -> bool:
-            return not DataTool.is_empty(PIH.SERVICE.ping(role))
+        def check_accessibility(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> bool:
+            role_descrption: ServiceRoleDescription = service_role_or_description if isinstance(
+                    service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+            return not DataTool.is_empty(PIH.SERVICE.ping(role_descrption))
 
         @staticmethod
-        def ping(role: ServiceRoles) -> ServiceRoleInformation:
-            service_role_informaion: ServiceRoleInformation = RPC.ping(role)
+        def ping(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> ServiceRoleInformation:
+            service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(
+                    service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+            service_role_informaion: ServiceRoleInformation = RPC.ping(service_role_or_description)
             if service_role_informaion is not None:
                 DataTool.fill_data_from_source(
-                    role.value, DataTool.to_data(service_role_informaion))
+                    service_role_description, service_role_informaion)
                 service_role_informaion.subscribers = list(map(lambda item: DataTool.fill_data_from_source(
                     Subscriber(), item), service_role_informaion.subscribers))
             return service_role_informaion
-
+        
         @staticmethod
         def init() -> None:
             if PIH.SERVICE.command_map is None:
                 PIH.SERVICE.command_map = {}
-                for role in ServiceRoles:
-                    for role_command in role.value.commands:
-                        PIH.SERVICE.command_map[role_command.name] = role
+                for service_role in ServiceRoles:
+                    service_role_description: ServiceRoleDescription = service_role.value
+                    for service_command in service_role_description.commands:
+                        PIH.SERVICE.command_map[service_command.name] = service_role_description
 
         @staticmethod
-        def get_role_by_command(value: ServiceCommands) -> ServiceRoles:
+        def get_role_description_by_command(value: ServiceCommands) -> ServiceRoleDescription:
             return PIH.SERVICE.command_map[value.name] if value.name in PIH.SERVICE.command_map else None
 
         @staticmethod
-        def get_host(service_role: ServiceRoles) -> str:
-            role_value: ServiceRoleDescription = service_role.value
-            if role_value.isolated:
-                host = PIH.OS.get_host()
-                role_value.host = host
-            return role_value.host
-
-        @staticmethod
-        def get_port(service_role: ServiceRoles) -> str:
-            role_value: ServiceRoleDescription = service_role.value
-            return role_value.port
-
-        @staticmethod
-        def subscribe_on(service_command: ServiceCommands, type: int = SubscribtionTypes.AFTER, name: str = None) -> bool:
-            return RPC.Service.subscribe_on(service_command, type, name)
+        def get_host(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> str:
+            service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+            if service_role_description.isolated:
+                service_role_description.host = PIH.OS.host()
+            return service_role_description.host
 
         @staticmethod
-        def unsubscribe(service_command: ServiceCommands, type: int) -> bool:
-            return RPC.Service.unsubscribe(service_command, type,)
+        def get_port(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> str:
+            service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+            return service_role_description.port
 
-    class PATH(PATHS):
+    class PATH(PATHS, PathTool):
 
         @staticmethod
         def resolve(value: str) -> str:
             if value[0] == "{" and value[-1] == "}":
                 value = value[1: -1]
-            return PathTool.resolve(value, PIH.OS.get_host())
+            return PathTool.resolve(value, PIH.OS.host())
+        
+        def join(path: str, *paths) -> str:
+            return os.path.join(path, *paths)
+        
+        class QR_CODE:
+
+            @staticmethod
+            def polibase_person_card_registry_folder(name: str) -> str:
+                name = PIH.DATA.FORMAT.polibase_person_card_registry_folder(name)
+                return os.path.join(PATHS.POLIBASE_APP_DATA.PERSON_CARD_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(name, FILE.EXTENSION.PNG)))
+
+            @staticmethod
+            def mobile_helper_command(name: str) -> str:
+                name = PIH.DATA.FORMAT.mobile_helper_command(name)
+                return os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(name, FILE.EXTENSION.PNG)))
+  
 
-    class DATA:
+    class DATA(DataTool, StringTool, ListTool, DateTimeTool, EnumTool):
 
+        @staticmethod
+        def save_base64_as_image(path: str, content: str) -> bool:
+            with open(path, "wb") as file:
+                file.write(base64.decodebytes(bytes(content, "utf-8")))
+                return True 
+            return False
+
+        @staticmethod
+        def uuid() -> str:
+            return str(uuid.uuid4().hex)
         
         @staticmethod
         def create_email(login: str) -> str:
             return "@".join((login, CONST.SITE_ADDRESS))
 
         @staticmethod
         def create_user_principal_name(login: str) -> str:
-            return "@".join((login, CONST.AD.DOMAIN_MAIN))
+            return "@".join((login, AD.DOMAIN_MAIN))
 
         class USER:
 
             @staticmethod
             def by_login(value: str) -> User:
                 return PIH.RESULT.USER.by_login(value).data
 
@@ -1992,61 +2185,90 @@
             @staticmethod
             def get(value: SETTINGS) -> Any:
                 return PIH.RESULT.SETTINGS.get(value).data
 
         class FILTER:
 
             @staticmethod
-            def users_by_dn(data: List[User], dn: str) -> List:
+            def symbols_only_in(value: str, check_value: str) -> str:
+                return "".join(c for c in value if c in check_value)
+
+            @staticmethod
+            def users_by_dn(data: list[User], dn: str) -> list:
                 return list(filter(lambda x: x.distinguishedName.find(dn) != -1, data))
 
         class EXTRACT:
 
             @staticmethod
+            def date(value: str, format: str) -> datetime | None:
+                result: datetime | None = None
+                try:
+                    result = DateTimeTool.from_string(value, format)
+                except ValueError as error:
+                    date_extract_pattern = "[0-9]{1,2}\\.[0-9]{1,2}\\.[0-9]{4}"
+                    date_list: list[str] = re.findall(date_extract_pattern, value)
+                    if not DataTool.is_empty(date_list):
+                        result = PIH.DATA.EXTRACT.date(date_list[0], format)
+                return result
+            
+            @staticmethod
             def wappi_telephone_number(value: any) -> str:
                 if isinstance(value, str):
                     return PIH.DATA.FORMAT.telephone_number(value.split(CONST.MESSAGE.WHATSAPP.WAPPI.CONTACT_SUFFIX)[0])
                 if isinstance(value, dict):
                     return PIH.DATA.FORMAT.telephone_number(value["user"])
 
-            @staticmethod
-            def whatsapp_message_from_service_command_parameter_list(parameter_list: ParameterList) -> WhatsAppMessage:
-                result: bool = parameter_list.next()
-                message: WhatsAppMessage = None
-                if result:
-                    message_parameters: list = parameter_list.next()
-                    message_command: LogCommands = LogCommands.WHATSAPP_MESSAGE_RECEIVED
-                    if EnumTool.get(LogCommands, message_parameters[0]) == message_command:
-                        param_item: ParamItem = message_command.value.params[0]
-                        message = DataTool.fill_data_from_source(
-                            WhatsAppMessage(), message_parameters[1][param_item.name])
-                return message
+            class SERVICE_PARAMETER_LIST:
+
+                @staticmethod
+                def whatsapp_message(parameter_list: ParameterList) -> WhatsAppMessage:
+                    result: bool = parameter_list.next()
+                    message: WhatsAppMessage = None
+                    if result:
+                        message_parameters: list[Any] = parameter_list.next()
+                        message_command: LogCommands = LogCommands.WHATSAPP_MESSAGE_RECEIVED
+                        if EnumTool.get(LogCommands, message_parameters[0]) == message_command:
+                            param_item: ParamItem = message_command.value.params[0]
+                            message = DataTool.fill_data_from_source(
+                                WhatsAppMessage(), message_parameters[1][param_item.name])
+                    return message
+                
+                @staticmethod
+                def log_command_parameters(parameter_list: ParameterList) -> tuple[LogCommands, list[Any]]:
+                    log_command_content: dict[str, Any] = parameter_list.list[1]
+                    log_command: LogCommands = EnumTool.get(LogCommands, log_command_content[0])
+                    log_command_parameters: dict[str, Any] = log_command_content[1]
+                    result: list[Any] = []
+                    if not A.D_C.empty(log_command.value.params):
+                        for log_command_parameters_description in log_command.value.params:
+                            result.append(log_command_parameters[log_command_parameters_description.name])
+                    return log_command, result
 
             @staticmethod
             def email(value: str) -> str:
-                emails: List[str] = re.findall(
+                emails: list[str] = re.findall(
                     r"[A-Za-z0-9_%+-.]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,5}", value)
                 if len(emails) > 0:
                     return emails[0]
                 return None
             
             @staticmethod
             def float(value: str) -> float:
                 if not DataTool.is_empty(value):
-                    floats: List[str] = re.findall(
+                    floats: list[str] = re.findall(
                         r"\d+[\.\,]*\d+", value)
                     if len(floats) > 0:
                         return float(floats[0].replace(",", "."))
                 return None
 
             @staticmethod
-            def number(value: str, min: int = None, max: int = None) -> int:
+            def decimal(value: str, min: int = None, max: int = None) -> int | None:
                 value = value.strip()
-                result: int = None
-                numbers: List[str] = re.findall(r"\d+", value)
+                result: int | None = None
+                numbers: list[str] = re.findall(r"\d+", value)
                 if len(numbers) > 0:
                     result = int(numbers[0])
                     if min is not None and max is not None and (result < min or result > max):
                         result = None
                 return result
 
             @staticmethod
@@ -2097,32 +2319,94 @@
             def mark_id(mark_object: dict) -> str:
                 return PIH.DATA.EXTRACT.parameter(mark_object, FIELD_NAME_COLLECTION.MARK_ID)
 
             @staticmethod
             def description(object: dict) -> str:
                 result = PIH.DATA.EXTRACT.parameter(
                     object, FIELD_NAME_COLLECTION.DESCRIPTION)
-                if isinstance(result, Tuple) or isinstance(result, List):
+                if isinstance(result, Tuple) or isinstance(result, list):
                     return result[0]
 
             @staticmethod
             def container_dn(user_object: dict) -> str:
                 return PIH.DATA.EXTRACT.container_dn_from_dn(PIH.DATA.EXTRACT.dn(user_object))
 
             @staticmethod
             def container_dn_from_dn(dn: str) -> str:
                 return ",".join(dn.split(",")[1:])
             
+        class CONVERT:
+
+            @staticmethod
+            def settings_to_datetime(item: SETTINGS, format: str = CONST.SECONDLESS_TIME_FORMAT) -> datetime | list[datetime]:
+                settings_value: str | list[str] = A.S.get(item)
+                return  PIH.DATA.CONVERT.settings_to_datetime_list(item, format) if isinstance(settings_value, list) else DateTimeTool.from_string(settings_value, format)
+            
+            @staticmethod
+            def settings_to_datetime_list(item: SETTINGS, format: str = CONST.SECONDLESS_TIME_FORMAT) -> list[datetime]:
+                return list(map( lambda item: DateTimeTool.from_string(item, format), A.S.get(item)))
+
+            @staticmethod
+            def file_to_base64(path: str) -> str | None:
+                with open(path, "rb") as file:
+                    return PIH.DATA.CONVERT.bytes_to_base64(file.read())
+                return None
+                
+            @staticmethod
+            def bytes_to_base64(value: bytes) -> str:
+                return PIH.DATA.CONVERT.bytes_to_string(PIH.DATA.CONVERT.to_base64(value))
+            
+            @staticmethod
+            def to_base64(value: Any) -> str:
+                return base64.b64encode(value)
+
+            @staticmethod 
+            def bytes_to_string(value: bytes) -> str:
+                return value.decode('utf-8')
+            
+            
         class CHECK:
 
-           pass
+            @staticmethod
+            def by_secondless_time(value_datetime: datetime, value_str: str) -> bool:
+                return False if DataTool.is_empty(value_str) else DateTimeTool.is_equal_by_time(value_datetime, DateTimeTool.from_string(value_str, CONST.SECONDLESS_TIME_FORMAT)) 
+            
+            @staticmethod
+            def empty(value) -> bool:
+                return DataTool.is_empty(value)
+
+            @staticmethod
+            def decimal(value: int | str) -> bool:
+                return isinstance(value, int) or (isinstance(value, str) and value.isdecimal())
 
         class FORMAT:
 
             @staticmethod
+            def by_name(value: str, data: Any) -> str | None:
+                if value == DATA.FORMATTER.MY_DATETIME:
+                    return PIH.DATA.FORMAT.datetime(data)
+                return None
+
+            @staticmethod
+            def polibase_person_card_registry_folder(value: str) -> str:
+                return value.upper()
+
+            @staticmethod
+            def mobile_helper_command(value: str) -> str:
+                return value.lower()
+
+            @staticmethod
+            def mobile_helper_qr_code_text(value: str) -> str:
+                return PIH.DATA.FORMAT.whatsapp_send_message_to(PIH.DATA.FORMAT.telephone_number_international(PIH.DATA.TELEPHONE_NUMBER.it_administrator()), f"{PIH.NAME} {value}".replace(" ", "+"))
+            
+            @staticmethod
+            def whatsapp_send_message_to(telephone_number: str, message: str) -> str:
+                return CONST.MESSAGE.WHATSAPP.SEND_MESSAGE_TO_TEMPLATE.format(telephone_number, message)
+
+            @staticmethod
             def string(value: str) -> str:
                 return ("" or value).lower().replace('"', '')
             
             @staticmethod
             def telephone_number(value: str, prefix: str = CONST.TELEPHONE_NUMBER_PREFIX) -> str:
                 if DataTool.is_empty(value):
                     return value
@@ -2152,69 +2436,73 @@
                 return PIH.DATA.FORMAT.telephone_number(value, CONST.INTERNATIONAL_TELEPHONE_NUMBER_PREFIX)
 
             @staticmethod
             def email(value: str) -> str:
                 return value.lower()
 
             @staticmethod
-            def name(value: str, remove_non_alpha: bool = False) -> str:
-                value_list: List[str] = list(
-                    filter(lambda item: len(item) > 0, value.split(" ")))
-                if len(value_list) == 1:
-                    if len(value) > 2:
-                        value = value[0].upper() + value[1:].lower()
-                    value = re.sub("[^а-яА-Яa-zA-Z]+", "",
+            def name(value: str, remove_non_alpha: bool = False, name_part_minimal_length: int | None = None) -> str:
+                name_part_list: list[str] = list(
+                    filter(lambda item: len(item) > (0 if name_part_minimal_length is None else name_part_minimal_length - 1), value.split(" ")))
+                if len(name_part_list) == 1:
+                    value = value.lower()
+                    value = re.sub("[^а-я]+", "",
                                    value) if remove_non_alpha else value
+                    if len(value) > 1:
+                        value = StringTool.capitalize(value)
                     return value
-                return " ".join(list(map(lambda item: PIH.DATA.FORMAT.name(item, remove_non_alpha), value_list)))
+                return " ".join(list(map(lambda item: PIH.DATA.FORMAT.name(item, remove_non_alpha), name_part_list)))
 
             @staticmethod
-            def location_list(value: str, remove_first: bool = True, reversed: bool = True) -> List[str]:
-                location_list: List[str] = value.split(
+            def location_list(value: str, remove_first: bool = True, reversed: bool = True) -> list[str]:
+                location_list: list[str] = value.split(
                     ",")[1 if remove_first else 0:]
                 if reversed:
                     location_list.reverse()
                 return list(map(
                     lambda item: item.split("=")[-1], location_list))
 
             @staticmethod
-            def get_user_account_control_values(uac: int) -> List[str]:
-                result: List[str] = []
-                for count, item in enumerate(CONST.AD.USER_ACCOUNT_CONTROL):
+            def get_user_account_control_values(uac: int) -> list[str]:
+                result: list[str] = []
+                for count, item in enumerate(AD.USER_ACCOUNT_CONTROL):
                     if (pow(2, count) & uac) != 0:
                         result.append(item)
                 return result
             
             @staticmethod
             def description(value: str) -> str:
                 return (value.split("|")[0]).rstrip()
+            
+            def datetime(iso_datetime_string: str) -> str:
+                return DateTimeTool.datetime_to_string(datetime.fromisoformat(iso_datetime_string), CONST.MY_DATE_FORMAT)
 
         class TELEPHONE_NUMBER:
 
             wappi_profile_TO_TELEPHONE_NUMBER_MAP: dict = None
 
             @staticmethod
-            def all(active: bool = True) -> List[str]:
+            def all(active: bool = True) -> list[str]:
                 def filter_function(user: User) -> str:
                     return user.telephoneNumber is not None
                 def map_function(user: User) -> str:
                     return PIH.DATA.FORMAT.telephone_number(user.telephoneNumber)
-                return ResultTool.map(ResultTool.filter(PIH.RESULT.USER.by_name(CONST.AD.SEARCH_ALL_PATTERN, active=active), filter_function), map_function).data
+                return ResultTool.map(ResultTool.filter(PIH.RESULT.USER.by_name(AD.SEARCH_ALL_PATTERN, active=active), filter_function), map_function).data
 
             @staticmethod
             def it_administrator() -> str:
-                return PIH.DATA.TELEPHONE_NUMBER.by_login(CONST.AD.ADMINISTRATOR)
+                return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.ADMINISTRATOR)
 
             @staticmethod
             def call_centre_administrator() -> str:
-                return PIH.DATA.TELEPHONE_NUMBER.by_login(CONST.AD.CALL_CENTRE_ADMINISTRATOR)
+                return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.CALL_CENTRE_ADMINISTRATOR)
 
             @staticmethod
             def marketer() -> str:
-                return PIH.DATA.TELEPHONE_NUMBER.by_login(CONST.AD.MARKETER)
+                return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.MARKETER)
 
             @staticmethod
             def for_wappi(value: Any) -> str:
                 WP = CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE
                 value = EnumTool.get_by_value_or_key(WP, value)
                 map: dict = PIH.DATA.TELEPHONE_NUMBER.wappi_profile_TO_TELEPHONE_NUMBER_MAP
                 if map is None:
@@ -2270,89 +2558,139 @@
         class POLIBASE:
 
             @staticmethod
             def person_by_pin(value: int, test: bool = None) -> PolibasePerson:
                 return PIH.RESULT.POLIBASE.person_by_pin(value, test).data
 
             @staticmethod
-            def duplicate_person_for(person: PolibasePerson, check_birth: bool = True) -> PolibasePerson:
+            def duplicate_persons_by_person(person: PolibasePerson, check_birth: bool = True) -> list[PolibasePerson]:
                 def check_function(check_person: PolibasePerson) -> bool:
-                    return check_person.pin != person.pin and (not check_birth or check_person.Birth != person.Birth)
+                    return check_person.pin != person.pin and (not check_birth or check_person.Birth == person.Birth)
                 return ResultTool.get_first_element(ResultTool.filter(PIH.RESULT.POLIBASE.persons_by_full_name(person.FullName), lambda item: check_function(item)))
+            
+            @staticmethod
+            def unique_by_telephone(value: str) -> PolibasePerson:
+                value = PIH.DATA.FORMAT.telephone_number(value)
+                def check_function(check_person: PolibasePerson) -> bool:
+                    return PIH.DATA.FORMAT.telephone_number(check_person.telephoneNumber) == value
+                return ResultTool.get_first_element(ResultTool.filter(PIH.RESULT.POLIBASE.person_by_telephone_number(value), lambda item: check_function(item)))
+
+            @staticmethod
+            def duplicate_persons_by_person_pin(value: int, check_birth: bool = True) -> list[PolibasePerson]:
+                try:
+                    return PIH.DATA.POLIBASE.duplicate_persons_by_person(PIH.RESULT.POLIBASE.person_by_pin(value).data, check_birth)
+                except NotFound as error:
+                    return None
 
             @staticmethod
-            def sort_person_list(value: List[PolibasePerson]) -> None:
+            def sort_person_list(value: list[PolibasePerson]) -> None:
                 value.sort(key=lambda item: item.pin)
 
     class OS:
 
         @staticmethod
         def get_login() -> str:
             return os.getlogin()
 
         @staticmethod
-        def get_host() -> str:
+        def host() -> str:
             return platform.node()
 
         @staticmethod
         def get_pid() -> int:
             return os.getppid()
 
-    class RESULT:
+    class RESULT(ResultTool):
+
+        class SSH:
+
+            @staticmethod
+            def execute(command: str, host: str, username: str | None = None, password: str | None = None) -> Result[list[str]]:
+                return DataTool.to_result(
+                    RPC.call(ServiceCommands.execute_ssh_command, (command, host, username, password)))
+
+            @staticmethod
+            def get_certificate_information(host: str, username: str | None = None, password: str | None = None) -> Result[str | None]:
+                return DataTool.to_result(
+                    RPC.call(ServiceCommands.get_certificate_information, (host, username, password)))
+            
+            @staticmethod
+            def get_unix_free_space_information_by_drive_name(drive_name: str, host: str, username: str | None = None, password: str | None = None) -> Result[str | None]:
+                return DataTool.to_result(
+                    RPC.call(ServiceCommands.get_unix_free_space_information_by_drive_name, (drive_name, host, username, password)))
 
         class DATA_STORAGE:
 
+            @staticmethod
             def value(name: str, class_type: T, section: str = None) -> Result[T]:
                 return DataTool.to_result(
                     RPC.call(ServiceCommands.get_storage_value, (name, section)), class_type)
+            
+            @staticmethod
+            def ogrn(code: str) -> Result[OGRN]:
+                return DataTool.to_result(
+                    RPC.call(ServiceCommands.get_ogrn_value, (code, )), OGRN)
+            
+            @staticmethod
+            def fms_unit_name(code: str) -> Result[str]:
+                return DataTool.to_result(
+                    RPC.call(ServiceCommands.get_fms_unit_name, (code, )))
 
         class MESSAGE:
 
             class DELAYED:
 
                 @staticmethod
-                def get(search_condition: MessageSearchCritery = None, take_to_work: bool = False) -> Result[List[DelayedMessageDS]]:
+                def get(search_condition: MessageSearchCritery = None, take_to_work: bool = False) -> Result[list[DelayedMessageDS]]:
                     return DataTool.to_result(
                         RPC.call(ServiceCommands.search_delayed_messages, (search_condition, take_to_work)), DelayedMessageDS)
 
         class RESOURCES:
 
             @staticmethod
-            def get_status_list(checkable_section_list: List[CheckableSections], force_update: bool = False, all: bool = False) -> Result[List[ResourceStatus]]:
+            def get_status_list(checkable_section_list: list[CheckableSections] = None, force_update: bool = False, all: bool = False) -> Result[list[ResourceStatus]]:
                 def get_type(data: dict) -> ResourceStatus:
                     if "check_certificate_status" in data:
                         return SiteResourceStatus()
                     return ResourceStatus()
                 return DataTool.to_result(RPC.call(ServiceCommands.get_resource_status_list, (None if DataTool.is_empty(checkable_section_list) else list(map(lambda item: item.name, checkable_section_list)), force_update, all)), get_type)
 
             @staticmethod
-            def get_status(resource_desription_or_address: Any, force: bool = False) -> ResourceStatus:
+            def get_resource_status_list(force_update: bool = False, all: bool = False) -> Result[list[ResourceStatus]]:
+                return PIH.RESULT.RESOURCES.get_status_list([CheckableSections.RESOURCES], force_update, all)
+
+            @staticmethod
+            def get_status(checkable_section_list: list[CheckableSections], resource_desription_or_address: Any, force: bool = False) -> ResourceStatus:
                 address: str = None
                 if isinstance(resource_desription_or_address, ResourceDescription):
                     address = resource_desription_or_address.address
                 elif isinstance(resource_desription_or_address, str):
                     address = resource_desription_or_address
                 if not DataTool.is_empty(address):
-                    resource_list: List[ResourceStatus] = PIH.RESULT.RESOURCES.get_status_list(force).data
+                    resource_list: list[ResourceStatus] = PIH.RESULT.RESOURCES.get_status_list(checkable_section_list, force).data
                     for item in resource_list:
                         if item.address == address:
                             return item
                 return None
             
+            @staticmethod
+            def get_resource_status(resource_desription_or_address: Any, force: bool = False) -> ResourceStatus:
+                return PIH.RESULT.RESOURCES.get_status([CheckableSections.RESOURCES], resource_desription_or_address, force)
+            
         class INDICATIONS:
 
             @staticmethod
-            def get_last_values(count: int = 1) -> Result[List[CTIndicationDS]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_last_ct_indications_value_list, (count, )), CTIndicationDS)
+            def get_last_items(count: int = 1) -> Result[list[CTIndicationItem]]:
+                return DataTool.to_result(RPC.call(ServiceCommands.get_last_ct_indications_value_list, (count, )), CTIndicationItem)
 
 
         class BACKUP:
 
             @staticmethod
-            def robocopy_status() -> Result[List[RobocopyJobStatus]]:
+            def robocopy_job_status_list() -> Result[list[RobocopyJobStatus]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.robocopy_get_job_status_list), RobocopyJobStatus)
 
         class SETTINGS:
 
             @staticmethod
             def key(key: str, default_value: Any = None) -> Result[Any]:
                 return DataTool.to_result(
@@ -2366,57 +2704,57 @@
         class SERVER:
 
             pass
 
         class WORKSTATION:
 
             @staticmethod
-            def all_description() -> Result[List[WorkstationDescription]]:
+            def all_description() -> Result[list[WorkstationDescription]]:
                 return DataTool.to_result(
                     RPC.call(ServiceCommands.get_all_workstation_description), WorkstationDescription)
 
             @staticmethod
-            def all_with_prooperty(value: CONST.AD.WSProperies) -> Result[List[Workstation]]:
+            def all_with_prooperty(value: AD.WSProperies) -> Result[list[Workstation]]:
                 def filter_function(workstation: Workstation) -> bool:
                     return BM.has(workstation.properties, value.value)
                 return ResultTool.filter(PIH.RESULT.WORKSTATION.all(), filter_function)
 
             @staticmethod
-            def by_login(value: str) -> Result[List[Workstation]]:
+            def by_login(value: str) -> Result[list[Workstation]]:
                 value = PIH.DATA.FORMAT.string(value)
                 if PIH.CHECK.USER.exists_by_login(value):
                     return DataTool.to_result(
                         RPC.call(ServiceCommands.get_workstation_by_user, value), Workstation)
                 else:
                     details: str = f"Пользователь с логином {value} не найден"
                     raise NotFound(details)
 
             @staticmethod
             def by_internal_telephone_number(value: int) -> Result[Workstation]:
-                result: Result[List[Workstation]] = PIH.RESULT.WORKSTATION.all()
-                workstation_list: List[Workstation] = result.data
+                result: Result[list[Workstation]] = PIH.RESULT.WORKSTATION.all()
+                workstation_list: list[Workstation] = result.data
                 result_worksation: Workstation = None
                 for workstation in workstation_list:
                     if not DataTool.is_empty(workstation.description):
                         index: int = workstation.description.find(CONST.INTERNAL_TELEPHONE_NUMBER_PREFIX)
                         if index != -1:
                             internal_telephone_number_text: str = workstation.description[index:]
-                            internal_telephone_number: int = PIH.DATA.EXTRACT.number(internal_telephone_number_text)
+                            internal_telephone_number: int = PIH.DATA.EXTRACT.decimal(internal_telephone_number_text)
                             if internal_telephone_number == value:
                                 result_worksation = workstation
                                 break
                 if result_worksation is not None:#and result_worksation.accessable and not DataTool.is_empty(result_worksation.samAccountName):
                     return Result(result.fields, workstation)
                 else:
                     raise PIH.ERROR.USER.get_not_found_error(
                         "внутренним номером телефона", True, str(value))
 
             @staticmethod
-            def by_any(value: Any) -> Result[List[Workstation]]:
-                if PIH.CHECK.number(value):
+            def by_any(value: Any) -> Result[list[Workstation]]:
+                if PIH.DATA.CHECK.decimal(value):
                     return ResultTool.as_list(PIH.RESULT.WORKSTATION.by_internal_telephone_number(int(value)))
                 if PIH.CHECK.WORKSTATION.name(value):
                     return ResultTool.as_list(PIH.RESULT.WORKSTATION.by_name(value))
                 try:
                     return PIH.RESULT.WORKSTATION.by_login(value)
                 except NotFound:
                     detail: str = f"Компьютер с параметром поиска {value} не найден"
@@ -2428,85 +2766,86 @@
                 result: Result[Workstation] = ResultTool.with_first_element(ResultTool.filter(
                     PIH.RESULT.WORKSTATION.all(), lambda item: item.name.lower() == value.lower()))
                 if ResultTool.is_empty(result):
                     raise NotFound(f"Компьютер с именем {value} не найден")
                 return result
 
             @staticmethod
-            def all() -> Result[List[Workstation]]:
+            def all() -> Result[list[Workstation]]:
                 def every_action(workstation: Workstation) -> None:
                     workstation.name = workstation.name.lower()
                 return ResultTool.every(DataTool.to_result(
                     RPC.call(ServiceCommands.get_all_workstations), Workstation), every_action)
 
         class INVENTORY:
 
             @staticmethod
-            def report(report_file_path: str, open_for_edit: bool = False) -> Result[List[InventoryReportItem]]:
+            def report(report_file_path: str, open_for_edit: bool = False) -> Result[list[InventoryReportItem]]:
                 return DataTool.to_result(
                     RPC.call(ServiceCommands.get_inventory_report, (report_file_path, open_for_edit)), InventoryReportItem)
 
         class TIME_TRACKING:
 
             @staticmethod
-            def today(tab_number: str = None) -> Result[List[TimeTrackingResultByPerson]]:
-                return PIH.RESULT.TIME_TRACKING.create(tab_number=tab_number)
+            def today(tab_number_list: list[str] = None) -> Result[list[TimeTrackingResultByPerson]]:
+                return PIH.RESULT.TIME_TRACKING.create(tab_number_list=tab_number_list)
+
+            def yesterday(tab_number_list: list[str] = None) -> Result[list[TimeTrackingResultByPerson]]:
+                yesterday: datetime = DateTimeTool.yesterday()
+                return PIH.RESULT.TIME_TRACKING.create(DateTimeTool.start_date(yesterday), DateTimeTool.start_date(yesterday), tab_number_list)
 
             @staticmethod
-            def in_period(day_start: int = 1, day_end: int = None, month: int = None, tab_number: str = None) -> Result[List[TimeTrackingResultByPerson]]:
+            def in_period(day_start: int = 1, day_end: int = None, month: int = None, tab_number: list[str] = None) -> Result[list[TimeTrackingResultByPerson]]:
                 now: datetime = datetime.now()
                 if month is not None:
                     now = now.replace(month=month)
-                start_date: datetime = now.replace(hour=0, minute=0, second=0)
-                end_date: datetime = now.replace(hour=23, minute=59, second=59)
+                start_date: datetime = DateTimeTool.start_date(now)
+                end_date: datetime = DateTimeTool.end_date(now)
                 if day_start < 0:
                     start_date -= timedelta(days=abs(day_start))
                 else:
                     start_date = start_date.replace(day=day_start)
                 if day_end is not None:
                     if day_end < 0:
                         day_end -= timedelta(days=abs(day_start))
                     else:
                         day_end = start_date.replace(day=day_start)
                 return PIH.RESULT.TIME_TRACKING.create(start_date, end_date, tab_number)
 
             @staticmethod
-            def create(start_date: datetime = None, end_date: datetime = None, tab_number: str = None) -> Result[List[TimeTrackingResultByPerson]]:
+            def create(start_date: datetime = None, end_date: datetime = None, tab_number_list: list[str] = None) -> Result[list[TimeTrackingResultByPerson]]:
                 now: datetime = datetime.now() if start_date is None or end_date is None else None
-                start_date = start_date or now.replace(
-                    hour=0, minute=0, second=0)
-                end_date = end_date or now.replace(
-                    hour=23, minute=59, second=59)
+                start_date = start_date or DateTimeTool.start_date(now)
+                end_date = end_date or DateTimeTool.end_date(now)
 
                 def get_date_or_time(entity: TimeTrackingEntity, date: bool) -> str:
-                    return DataTool.not_none_check(entity, lambda: entity.TimeVal.split("T")[not date])
+                    return DataTool.not_none_check(entity, lambda: entity.TimeVal.split(CONST.DATE_TIME_SPLITTER)[not date])
                 result_data: dict = {}
                 full_name_by_tab_number_map: dict = {}
-                result_data = defaultdict(
-                    lambda: defaultdict(lambda: defaultdict(list)))
-                data: List = DataTool.to_result(RPC.call(
-                    ServiceCommands.get_time_tracking, (start_date, end_date, tab_number)), TimeTrackingEntity).data
+                result_data = defaultdict(lambda: defaultdict(lambda: defaultdict(list)))
+                data: list[TimeTrackingEntity] = DataTool.to_result(RPC.call(
+                    ServiceCommands.get_time_tracking, (start_date, end_date, tab_number_list)), TimeTrackingEntity).data
                 for time_tracking_entity in data:
                     tab_number: str = time_tracking_entity.TabNumber
                     full_name_by_tab_number_map[tab_number] = time_tracking_entity.FullName
                     result_data[time_tracking_entity.DivisionName][tab_number][get_date_or_time(time_tracking_entity, True)].append(
                         time_tracking_entity)
-                result: List[TimeTrackingResultByDivision] = []
+                result: list[TimeTrackingResultByDivision] = []
                 for division_name in result_data:
                     if division_name is None:
                         continue
                     result_division_item: TimeTrackingResultByDivision = TimeTrackingResultByDivision(
                         division_name)
                     result.append(result_division_item)
                     for tab_number in result_data[division_name]:
                         result_person_item: TimeTrackingResultByPerson = TimeTrackingResultByPerson(
                             tab_number, full_name_by_tab_number_map[tab_number])
                         result_division_item.list.append(result_person_item)
                         for date in result_data[division_name][tab_number]:
-                            time_tracking_entity_list: List[TimeTrackingEntity] = result_data[division_name][tab_number][date]
+                            time_tracking_entity_list: list[TimeTrackingEntity] = result_data[division_name][tab_number][date]
                             time_tracking_enter_entity: TimeTrackingEntity = None
                             time_tracking_exit_entity: TimeTrackingEntity = None
                             for time_tracking_entity_list_item in time_tracking_entity_list:
                                 if time_tracking_entity_list_item.Mode == 1:
                                     time_tracking_enter_entity = time_tracking_entity_list_item
                                 if time_tracking_entity_list_item.Mode == 2:
                                     time_tracking_exit_entity = time_tracking_entity_list_item
@@ -2524,52 +2863,52 @@
                                     result_person_item.duration += duration
                             result_person_item.list.append(
                                 TimeTrackingResultByDate(date, get_date_or_time(time_tracking_enter_entity, False),
                                                          get_date_or_time(time_tracking_exit_entity, False), duration))
                 for division in result:
                     for person in division.list:
                         index: int = 0
-                        length = len(person.list)
+                        length: int = len(person.list)
                         for _ in range(length):
                             item: TimeTrackingResultByDate = person.list[index]
                             if item.duration == 0:
                                 # if item.enter_time is None and item.exit_time is not None:
                                 if index < length - 1:
                                     item_next: TimeTrackingResultByDate = person.list[index + 1]
                                     if item.exit_time is not None:
                                         if item_next.enter_time is not None:
-                                            duration = int(datetime.fromisoformat(item.date + "T" + item.exit_time).timestamp(
-                                            ) - datetime.fromisoformat(item_next.date + "T" + item_next.enter_time).timestamp())
+                                            duration = int(datetime.fromisoformat(item.date + CONST.DATE_TIME_SPLITTER + item.exit_time).timestamp(
+                                            ) - datetime.fromisoformat(item_next.date + CONST.DATE_TIME_SPLITTER + item_next.enter_time).timestamp())
                                             item.duration = duration
                                             person.duration += duration
                                             if item_next.exit_time is None:
                                                 index += 1
                             index += 1
                             if index >= length - 1:
                                 break
 
                 return Result(FIELD_COLLECTION.ORION.TIME_TRACKING_RESULT, result)
 
         class PRINTER:
 
             @staticmethod
-            def all() -> Result[List[PrinterADInformation]]:
-                def filter_by_server_name(printer_list: List[PrinterADInformation]) -> List[PrinterADInformation]:
+            def all() -> Result[list[PrinterADInformation]]:
+                def filter_by_server_name(printer_list: list[PrinterADInformation]) -> list[PrinterADInformation]:
                     return list(filter(lambda item: item.serverName == CONST.HOST.PRINTER_SERVER.NAME, printer_list))
-                result: Result[List[PrinterADInformation]] = DataTool.to_result(
+                result: Result[list[PrinterADInformation]] = DataTool.to_result(
                     RPC.call(ServiceCommands.get_printers), PrinterADInformation)
                 return Result(result.fields, filter_by_server_name(result.data))
 
             @staticmethod
-            def report(redirect_to_log: bool = True) -> Result[List[PrinterReport]]:
+            def report(redirect_to_log: bool = True) -> Result[list[PrinterReport]]:
                 return DataTool.to_result(
                     RPC.call(ServiceCommands.printers_report, redirect_to_log), PrinterReport)
 
             @staticmethod
-            def status(redirect_to_log: bool = True) -> Result[List[PrinterStatus]]:
+            def status(redirect_to_log: bool = True) -> Result[list[PrinterStatus]]:
                 return DataTool.to_result(
                     RPC.call(ServiceCommands.printers_status, redirect_to_log), PrinterStatus)
 
         class MARK:
 
             @staticmethod
             def by_tab_number(value: str) -> Result[Mark]:
@@ -2577,56 +2916,56 @@
                     RPC.call(ServiceCommands.get_mark_by_tab_number, value), Mark)
                 if ResultTool.is_empty(result):
                     details: str = f"Карта доступа с номером '{value}' не найдена"
                     raise NotFound(details)
                 return result
 
             @staticmethod
-            def person_divisions() -> Result[List[Mark]]:
+            def person_divisions() -> Result[list[Mark]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_person_divisions), MarkDivision)
 
             @staticmethod
-            def by_name(value: str, first_item: bool = False) -> Result[List[Mark]]:
+            def by_name(value: str, first_item: bool = False) -> Result[list[Mark]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_mark_by_person_name, value), Mark, first_item)
 
             @staticmethod
-            def by_full_name(value: FullName, first_item: bool = False) -> Result[List[Mark]]:
+            def by_full_name(value: FullName, first_item: bool = False) -> Result[list[Mark]]:
                 return PIH.RESULT.MARK.by_name(FullNameTool.from_string(value), first_item)
 
             @staticmethod
-            def temporary_list() -> Result[List[TemporaryMark]]:
+            def temporary_list() -> Result[list[TemporaryMark]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_temporary_marks), TemporaryMark)
 
             @staticmethod
-            def by_any(value: str) -> Result[List[Mark]]:
+            def by_any(value: str) -> Result[list[Mark]]:
                 if PIH.CHECK.MARK.tab_number(value):
                     return ResultTool.as_list(PIH.RESULT.MARK.by_tab_number(value))
                 elif PIH.CHECK.name(value, True):
                     return PIH.RESULT.MARK.by_name(value)
                 return Result()
 
             @staticmethod
-            def free_list(show_with_guest_marks: bool = False) -> Result[List[Mark]]:
-                result: Result[List[Mark]] = DataTool.to_result(
+            def free_list(show_with_guest_marks: bool = False) -> Result[list[Mark]]:
+                result: Result[list[Mark]] = DataTool.to_result(
                     RPC.call(ServiceCommands.get_free_marks), Mark)
 
                 def filter_function(item: Mark) -> bool:
                     return EnumTool.get(MarkType, item.type) != MarkType.GUEST
                 return result if show_with_guest_marks else ResultTool.filter(result, filter_function)
 
             @staticmethod
-            def free_marks_by_group_id(value: int) -> Result[List[Mark]]:
+            def free_marks_by_group_id(value: int) -> Result[list[Mark]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_free_marks_by_group_id, value), Mark)
 
             @staticmethod
-            def free_marks_group_statistics(show_guest_marks: bool = None) -> Result[List[MarkGroupStatistics]]:
+            def free_marks_group_statistics(show_guest_marks: bool = None) -> Result[list[MarkGroupStatistics]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_free_marks_group_statistics, show_guest_marks), MarkGroupStatistics)
 
             @staticmethod
-            def all() -> Result[List[Mark]]:
+            def all() -> Result[list[Mark]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_all_persons), Mark)
 
             @staticmethod
             def temporary_mark_owner(mark: Mark) -> Result[Mark]:
                 return DataTool.check(mark is not None and EnumTool.get(MarkType, mark.type) == MarkType.TEMPORARY, lambda: DataTool.to_result(RPC.call(ServiceCommands.get_owner_mark_for_temporary_mark, mark.TabNumber), Mark), None)
 
             @staticmethod
@@ -2634,15 +2973,15 @@
                 return PIH.RESULT.MARK.temporary_mark_owner(PIH.RESULT.MARK.by_tab_number(value).data)
 
         class POLIBASE:
 
             class NOTIFICATION:
 
                 @staticmethod
-                def by(value: PolibasePersonVisitNotification) -> Result[List[PolibasePersonVisitNotification]]:
+                def by(value: PolibasePersonVisitNotification) -> Result[list[PolibasePersonVisitNotification]]:
                     return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visit_notifications, value), PolibasePersonVisitNotification)
 
                 @staticmethod
                 def by_message_id(value: int) -> Result[PolibasePersonVisitNotification]:
                     return ResultTool.with_first_element(PIH.RESULT.POLIBASE.NOTIFICATION.by(PolibasePersonVisitNotification(messageID=value)))
 
                 class CONFIRMATION:
@@ -2650,46 +2989,46 @@
                     @staticmethod
                     def by(recipient: str, sender: str) -> Result[PolibasePersonNotificationConfirmation]:
                         return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_notification_confirmation, PolibasePersonNotificationConfirmation(recipient, sender)), PolibasePersonNotificationConfirmation)
 
             class INFORMATION_QUEST:
 
                 @staticmethod
-                def get(search_critery: PolibasePersonInformationQuest) -> Result[List[PolibasePersonInformationQuest]]:
+                def get(search_critery: PolibasePersonInformationQuest) -> Result[list[PolibasePersonInformationQuest]]:
                     return DataTool.to_result(
                         RPC.call(ServiceCommands.search_polibase_person_information_quests, search_critery), PolibasePersonInformationQuest)
 
             class VISIT:
 
                 @staticmethod
-                def after_id(value: int, test: bool = None) -> Result[List[PolibasePersonVisitDS]]:
+                def after_id(value: int, test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
                     return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visits, (PolibasePersonVisitSearchCritery(vis_no=f">{value}"), test)), PolibasePersonVisitDS)
 
                 @staticmethod
                 def by_id(value: int, test: bool = None) -> Result[PolibasePersonVisitDS]:
                     return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visits, (PolibasePersonVisitSearchCritery(vis_no=value), test)), PolibasePersonVisitDS, True)
 
                 @staticmethod
                 def last_id(test: bool = None) -> Result[int]:
                     return DataTool.to_result(RPC.call(ServiceCommands.get_polibase_person_visits_last_id, test))
 
                 @staticmethod
-                def today(test: bool = None) -> Result[List[PolibasePersonVisitDS]]:
+                def today(test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
                     return PIH.RESULT.POLIBASE.VISIT.by_registration_date(DateTimeTool.today(), test)
 
                 @staticmethod
-                def prerecording_today(test: bool = None) -> Result[List[PolibasePersonVisitDS]]:
+                def prerecording_today(test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
                     return PIH.RESULT.POLIBASE.VISIT.prerecording_by_registration_date(DateTimeTool.today(), test)
 
                 @staticmethod
-                def by_registration_date(value: datetime, test: bool = None) -> Result[List[PolibasePersonVisitDS]]:
+                def by_registration_date(value: datetime, test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
                     return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visits, (PolibasePersonVisitSearchCritery(vis_reg_date=DateTimeTool.date_to_string(value, CONST.POLIBASE.DATE_FORMAT)), test)), PolibasePersonVisitDS)
 
                 @staticmethod
-                def prerecording_by_registration_date(value: datetime = None, test: bool = None) -> Result[List[PolibasePersonVisitDS]]:
+                def prerecording_by_registration_date(value: datetime = None, test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
                     def filter_function(value: PolibasePersonVisitDS) -> bool:
                         return value.pin == CONST.POLIBASE.PRERECORDING_PIN
                     return ResultTool.filter(PIH.RESULT.POLIBASE.VISIT.by_registration_date(value, test), filter_function)
 
                 class DATA_STORAGE:
 
                     @staticmethod
@@ -2697,15 +3036,15 @@
                         return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visits_in_data_storage, (value, )), PolibasePersonVisitDS, True)
 
                     @staticmethod
                     def last() -> Result[PolibasePersonVisitDS]:
                         return PIH.RESULT.POLIBASE.VISIT.DATA_STORAGE.search(PolibasePersonVisitDS(id=-1))
 
 
-            def person_by_telephone_number(value: str, test: bool = None) -> Result[List[PolibasePerson]]:
+            def person_by_telephone_number(value: str, test: bool = None) -> Result[list[PolibasePerson]]:
                 value = PIH.DATA.FORMAT.telephone_number_international(value)
                 result: Result[PolibasePerson] = DataTool.to_result(RPC.call(
                     ServiceCommands.get_polibase_persons_by_telephone_number, (value, test)), PolibasePerson)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error("идентификационным номером", value)
                 return result
 
@@ -2714,51 +3053,53 @@
                 result: Result[PolibasePerson] = DataTool.to_result(RPC.call(
                     ServiceCommands.get_polibase_person_by_pin, (value, test)), PolibasePerson)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error("идентификационным номером", value)
                 return result
 
             @staticmethod
-            def persons_pin_by_visit_date(date: datetime, test: bool = None) -> Result[List[int]]:
+            def persons_pin_by_visit_date(date: datetime, test: bool = None) -> Result[list[int]]:
                 if test:
                     return Result(None, [100310])
                 return DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_pin_by_visit_date, (date.strftime(CONST.DATE_FORMAT), test)))
 
             @staticmethod
             def person_creator_by_pin(value: int, test: bool = None) -> Result[PolibasePerson]:
-                result: Result[List[PolibasePerson]] = DataTool.to_result(RPC.call(ServiceCommands.get_polibase_person_registrator_by_pin, (value, test)), PolibasePerson)
+                result: Result[list[PolibasePerson]] = DataTool.to_result(RPC.call(ServiceCommands.get_polibase_person_registrator_by_pin, (value, test)), PolibasePerson)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error(
                         "идентификационным номером", value)
                 return result
 
             @staticmethod
-            def persons_by_full_name(value: str, test: bool = None) -> Result[List[PolibasePerson]]:
-                result: Result[List[PolibasePerson]] = DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_by_full_name, (value, test)), PolibasePerson)
+            def persons_by_full_name(value: str, test: bool = None) -> Result[list[PolibasePerson]]:
+                result: Result[list[PolibasePerson]] = DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_by_full_name, (value, test)), PolibasePerson)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error("именем", value)
                 return result
 
             @staticmethod
-            def persons_by_pin(value: List[int], test: bool = None) -> Result[List[PolibasePerson]]:
-                result: Result[List[PolibasePerson]] = DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_by_pin, (value, test)), PolibasePerson)
+            def persons_by_pin(value: list[int], test: bool = None) -> Result[list[PolibasePerson]]:
+                result: Result[list[PolibasePerson]] = DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_by_pin, (value, test)), PolibasePerson)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error("идентификационным номером", value)
                 return result
 
             @staticmethod
-            def persons_by_card_registry_folder_name(value: str, test: bool = None) -> Result[List[PolibasePerson]]:
+            def persons_by_card_registry_folder_name(value: str, test: bool = None) -> Result[list[PolibasePerson]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_by_card_registry_folder_name, (value, test)), PolibasePerson)
 
             @staticmethod
-            def person_pin_list_with_old_format_barcode(test: bool = None) -> Result[List[int]]:
+            def person_pin_list_with_old_format_barcode(test: bool = None) -> Result[list[int]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_polibase_person_pin_list_with_old_format_barcode, (test, )))
 
             @staticmethod
-            def persons_by_any(value: str, test: bool = None) -> Result[List[PolibasePerson]]:
+            def persons_by_any(value: str, test: bool = None) -> Result[list[PolibasePerson]]:
+                if PIH.CHECK.telephone_number(value) or PIH.CHECK.telephone_number_international(value):
+                    return ResultTool.as_list(PIH.RESULT.POLIBASE.person_by_telephone_number(value, test))
                 if PIH.CHECK.POLIBASE.person_pin(value):
                     return ResultTool.as_list(PIH.RESULT.POLIBASE.person_by_pin(int(value), test))
                 if PIH.CHECK.POLIBASE.person_card_registry_folder_name(value):
                     return PIH.RESULT.POLIBASE.persons_by_card_registry_folder_name(value, test)
                 return ResultTool.as_list(PIH.RESULT.POLIBASE.persons_by_full_name(value))
 
         class USER:
@@ -2783,15 +3124,15 @@
                 workstation_list: list[Workstation] = PIH.RESULT.WORKSTATION.all().data
                 result_worksation: Workstation = None
                 for workstation in workstation_list:
                     if not DataTool.is_empty(workstation.description):
                         index: int = workstation.description.find(CONST.INTERNAL_TELEPHONE_NUMBER_PREFIX)
                         if index != -1:
                             internal_telephone_number_text: str = workstation.description[index:]
-                            internal_telephone_number: int = PIH.DATA.EXTRACT.number(internal_telephone_number_text)
+                            internal_telephone_number: int = PIH.DATA.EXTRACT.decimal(internal_telephone_number_text)
                             if internal_telephone_number == value:
                                 result_worksation = workstation
                                 break
                 if result_worksation is not None and result_worksation.accessable and not DataTool.is_empty(result_worksation.samAccountName):
                     return PIH.RESULT.USER.by_login(workstation.samAccountName)
                 else:
                     raise PIH.ERROR.USER.get_not_found_error(
@@ -2810,16 +3151,16 @@
                     details: str = f"Компьютер с именем '{name}' не найден!"
                     raise NotFound(details)
                 if user_workstation.samAccountName is None:
                     raise NotFound(f"За компьютером {name} нет залогиненного пользователя", name)
                 return PIH.RESULT.USER.by_login(user_workstation.samAccountName)
 
             @staticmethod
-            def by_any(value: Any, active: bool = None) -> Result[List[User]]:
-                def by_number(value: int) -> Result[List[User]]:
+            def by_any(value: Any, active: bool = None) -> Result[list[User]]:
+                def by_number(value: int) -> Result[list[User]]:
                     try:
                         return ResultTool.as_list(PIH.RESULT.USER.by_tab_number(value))
                     except NotFound:
                         try:
                             return ResultTool.as_list(PIH.RESULT.USER.by_login(PIH.RESULT.WORKSTATION.by_internal_telephone_number(value).data.samAccountName))
                         except:
                             return ResultTool.as_list(PIH.RESULT.USER.by_polibase_pin(value))
@@ -2835,69 +3176,69 @@
                         return PIH.RESULT.USER.by_group_name(value)
                     try:
                         value_as_telephone_number: str = PIH.DATA.FORMAT.telephone_number(value)
                         if PIH.CHECK.telephone_number(value_as_telephone_number):
                             return ResultTool.as_list(PIH.RESULT.USER.by_telephone_number(value_as_telephone_number, active))
                     except Exception:
                         pass
-                    if PIH.CHECK.number(value):
+                    if PIH.DATA.CHECK.decimal(value):
                        return by_number(value)
                     if PIH.CHECK.WORKSTATION.name(value):
                         return ResultTool.as_list(PIH.RESULT.USER.by_workstation_name(value))
                     if PIH.CHECK.login(value):
                         return ResultTool.as_list(PIH.RESULT.USER.by_login(value, active))
                     if value == "" or PIH.CHECK.name(value):
                         return PIH.RESULT.USER.by_name(value, active)
                 elif isinstance(value, int):
                     return by_number(value)
                 raise PIH.ERROR.USER.get_not_found_error("поисковым значением", active, value)
 
             @staticmethod
-            def by_job_position(value: CONST.AD.JobPisitions) -> Result[List[User]]:
+            def by_job_position(value: AD.JobPisitions) -> Result[list[User]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_users_by_job_position, value.name), User)
 
             @staticmethod
-            def by_group(value: CONST.AD.Groups) -> Result[List[User]]:
+            def by_group(value: AD.Groups) -> Result[list[User]]:
                 return PIH.RESULT.USER.by_group_name(value.name)
 
             @staticmethod
-            def by_group_name(value: str) -> Result[List[User]]:
+            def by_group_name(value: str) -> Result[list[User]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_users_by_group, value), User)
 
 
             @staticmethod
-            def template_list() -> Result[List[User]]:
+            def template_list() -> Result[list[User]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_template_users), User)
 
             @staticmethod
-            def containers() -> Result[List[UserContainer]]:
+            def containers() -> Result[list[UserContainer]]:
                 return DataTool.to_result(RPC.call(
                     ServiceCommands.get_containers), UserContainer)
 
             @staticmethod
-            def by_full_name(value: FullName, get_first: bool = False, active: bool = None) -> Result[List[User]]:
+            def by_full_name(value: FullName, get_first: bool = False, active: bool = None) -> Result[list[User]]:
                 return DataTool.to_result(RPC.call(ServiceCommands.get_user_by_full_name, (value, active)), User, get_first)
 
             @staticmethod
-            def by_name(value: str, active: bool = None) -> Result[List[User]]:
-                result: Result[List[User]] = DataTool.to_result(
+            def by_name(value: str, active: bool = None) -> Result[list[User]]:
+                result: Result[list[User]] = DataTool.to_result(
                     RPC.call(ServiceCommands.get_users_by_name, (value, active)), User)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.USER.get_not_found_error("именем", active, value)
                 return result
 
             @staticmethod
-            def list(active: bool = None) -> Result[List[User]]:
-                return PIH.RESULT.USER.by_name(CONST.AD.SEARCH_ALL_PATTERN, active)
+            def all(active: bool = None) -> Result[list[User]]:
+                return PIH.RESULT.USER.by_name(AD.SEARCH_ALL_PATTERN, active)
 
             @staticmethod
-            def list_with_telephone_number(active: bool = None) -> Result[List[User]]:
+            def list_with_telephone_number(active: bool = None) -> Result[list[User]]:
                 def user_with_telephone_number(user: User) -> bool:
                     return PIH.CHECK.telephone_number(user.telephoneNumber)
-                return ResultTool.filter(PIH.RESULT.USER.list(active), lambda user: user_with_telephone_number(user))
+                return ResultTool.filter(PIH.RESULT.USER.all(active), lambda user: user_with_telephone_number(user))
 
             @staticmethod
             def by_tab_number(value: str) -> Result[User]:
                 result: Result[Mark] = PIH.RESULT.MARK.by_tab_number(value)
                 if ResultTool.is_empty(result):
                     details: str = f"Карта доступа с номером {value} не найдена"
                     raise NotFound(details)
@@ -2905,20 +3246,37 @@
 
             @staticmethod
             def by_mark(value: Mark) -> Result[User]:
                 return Result(FIELD_COLLECTION.AD.USER, DataTool.check(value, lambda: DataTool.get_first_item(PIH.RESULT.USER.by_full_name(FullNameTool.from_string(value.FullName)).data)))
 
     class CHECK:
 
-        class RESOURCE_MANAGER:
+        class SETTINGS:
+    
+            @staticmethod
+            def by_time(current: datetime, settings: SETTINGS) -> bool:
+                return DateTimeTool.is_equal_by_time(current, PIH.SETTINGS.to_datetime(settings))
+
+        class INDICATION:
+
+            @staticmethod
+            def ct_notification_start_time(current: datetime) -> bool:
+                start_time_list: list[datetime] = PIH.SETTINGS.INDICATION.ct_notification_start_time()
+                for start_time in start_time_list:
+                    if DateTimeTool.is_equal_by_time(current, start_time):
+                        return True
+                return False
+
+        class RESOURCE:
         
             @staticmethod
-            def accessibility_by_ping(address: str, host: str = None, count: int = None, check_for_all: bool = True) -> bool:
+            def accessibility_by_ping(address_or_ip: str, host: str = None, count: int = None, check_for_all: bool = True) -> bool:
                 count = count or 4
-                local_ping_commnad_list: list[str] = [PIH.PSTOOLS.get_executor_path("psping"), "-accepteula", "-4", "-n", str(count), address]
+                local_ping_commnad_list: list[str] = [PIH.PSTOOLS.get_executor_path(
+                    CONST.PSTOOLS.PS_PING), CONST.PSTOOLS.ACCEPTEULA, "-4", "-n", str(count), address_or_ip]
                 pocess_result: CompletedProcess = A.PS.execute_command_list(local_ping_commnad_list if host is None else A.PS.create_command_list_for_psexec_command(local_ping_commnad_list, host, interactive=True), True, True)
                 if pocess_result.returncode == 0:
                     out: str = pocess_result.stdout
                     lost_marker: str = "Lost = "
                     index: int = out.find(lost_marker)
                     if index != -1:
                         lost_count: int = int(out[index +
@@ -2930,132 +3288,131 @@
 
             @staticmethod
             def accessibility(resource_status_or_address: Any) -> bool:
                 resource_status: ResourceStatus = None
                 if isinstance(resource_status_or_address, ResourceDescription):
                     resource_status = resource_status_or_address
                 else:
-                    resource_status = PIH.RESULT.RESOURCES.get_status(resource_status_or_address)
+                    resource_status = PIH.RESULT.RESOURCES.get_resource_status(
+                        resource_status_or_address)
                 return None if resource_status is None else resource_status.inaccessibility_counter < resource_status.inaccessibility_check_values[0]
                 
             @staticmethod
             def vpn_pacs_accessibility(count: int = 2) -> bool:
-                return PIH.CHECK.RESOURCE_MANAGER.accessibility_by_ping(RESOURCE_DESCRIPTION_COLLECTION.VPN_PACS.address, CONST.HOST.WS255.NAME, count)
+                return PIH.PSTOOLS.ping(RESOURCE.DESCRIPTIONS.VPN_PACS_SPB.address, CONST.HOST.WS255.NAME, count)
             
             @staticmethod
-            def PACS_accessibility(count: int = 2) -> bool:
-                return PIH.CHECK.RESOURCE_MANAGER.accessibility_by_ping(RESOURCE_DESCRIPTION_COLLECTION.PACS.address, CONST.HOST.WS255.NAME, count)
+            def pacs_accessibility(count: int = 2) -> bool:
+                return PIH.CHECK.RESOURCE.accessibility_by_ping(RESOURCE.DESCRIPTIONS.PACS_SPB.address, CONST.HOST.WS255.NAME, count)
            
             @staticmethod
             def wappi_profile_accessibility(value: Any, cached: bool = False) -> bool:
-                return PIH.CHECK.RESOURCE_MANAGER.accessibility(PIH.RESULT.RESOURCES.get_status(EnumTool.get_value(value, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value))) if cached else PIH.CHECK.MESSAGE.WHATSAPP.WAPPI.accessibility(value, False) 
+                return PIH.CHECK.RESOURCE.accessibility(PIH.RESULT.RESOURCES.get_resource_status(EnumTool.get_value(value, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value))) if cached else PIH.CHECK.MESSAGE.WHATSAPP.WAPPI.accessibility(value, False)
 
             @staticmethod
             def ws_accessibility(name: str) -> bool:
                 result: Result[Workstation] = PIH.RESULT.WORKSTATION.by_name(name)
                 return not ResultTool.is_empty(result) and result.data.accessable
             
             @staticmethod
-            def polibase_accessibility() -> bool:
+            def polibase_accessibility(cached: bool = False) -> bool:
                 try:
-                    return PIH.SERVICE.check_accessibility(ServiceRoles.POLIBASE) and PIH.CHECK.POLIBASE.person_exists_by_pin(CONST.POLIBASE.PRERECORDING_PIN)
+                    if cached:
+                        return PIH.RESULT.RESOURCES.get_resource_status(RESOURCE.DESCRIPTIONS.POLIBASE).accessable
+                    result_by_ping: bool = PIH.SERVICE.check_accessibility(ServiceRoles.POLIBASE)    
+                    result_by_pin : bool = PIH.CHECK.POLIBASE.person_exists_by_pin(CONST.POLIBASE.PRERECORDING_PIN)
+                    print("POLIBASE", result_by_ping, result_by_pin)
+                    return result_by_ping and result_by_pin
                 except NotFound:
+                    print("POLIBASE BY PIN")
                     pass
                 return False
 
-        @staticmethod
-        def email_accessability(value: str) -> bool:
-            return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_email_accessibility, value))
+        class EMAIL:
 
-        @staticmethod
-        def number(value: Any) -> bool:
-            return isinstance(value, int) or value.isdecimal()
+            @staticmethod
+            def accessability(value: str) -> bool:
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_email_accessibility, value))
 
         class FILE:
 
             @staticmethod
             def excel_file(path: str) -> bool:
                 return os.path.isfile(path) and PathTool.get_extension(path) in [FILE.EXTENSION.EXCEL_OLD, FILE.EXTENSION.EXCEL_NEW]
 
         class ACCESS:
 
             @staticmethod
-            def by_group(group: CONST.AD.Groups, exit_on_access_denied: bool = False, session: SessionBase = None, notify_on_fail: bool = True, notify_on_success: bool = True) -> bool:
+            def by_group(group: AD.Groups, exit_on_access_denied: bool = False, session: SessionBase = None, notify_on_fail: bool = True, notify_on_success: bool = True) -> bool:
                 session = session or PIH.session
-                login: str = session.get_login()
+                user: User = session.get_user()
                 result: bool = False
-                notify: bool = True
+                notify: bool = notify_on_success or notify_on_fail
                 if group in session.allowed_groups:
                     result = True
                     notify = False
                 else:
-                    user_list: List[User] = PIH.RESULT.USER.by_group(
-                        group).data
-                    if user_list is not None:
-                        for user_item in user_list:
-                            user: User = user_item
-                            if user.samAccountName == login:
-                                session.add_allowed_group(group)
-                                result = True
-                                break
-                if notify:
-                    if (result and notify_on_success) or (not result and notify_on_fail):
-                        PIH.LOG.from_service_bot(
-                            f"Запрос на доступа к группе: {group.name} от пользователя {session.get_user().name} ({login}). Доступ {'разрешен' if result else 'отклонен'}.", LogLevels.NORMAL if result else LogLevels.ERROR)
-                if exit_on_access_denied:
+                    result = PIH.CHECK.USER.by_group(user, group)
                     if result:
-                        return result
+                        session.add_allowed_group(group)
+                if notify:
+                    PIH.LOG.it(
+                        f"Запрос на доступа к группе: {group.name} от пользователя {user.name} ({user.samAccountName}). Доступ {'разрешен' if result else 'отклонен'}.", LogLevels.NORMAL if result else LogLevels.ERROR)
+                if not result and exit_on_access_denied:
                     session.exit(5, "Функционал недоступен...")
-                else:
-                    return result
+                return result
 
             @staticmethod
             def admin(exit_on_access_denied: bool = False, session: SessionBase = None, notify_on_fail: bool = True, notify_on_success: bool = True) -> bool:
-                return PIH.CHECK.ACCESS.by_group(CONST.AD.Groups.Admin, exit_on_access_denied, session, notify_on_fail, notify_on_success)
+                return PIH.CHECK.ACCESS.by_group(AD.Groups.Admin, exit_on_access_denied, session, notify_on_fail, notify_on_success)
 
             @staticmethod
             def service_admin(session: SessionBase = None, notify_on_fail: bool = True, notify_on_success: bool = True) -> bool:
-                return PIH.CHECK.ACCESS.by_group(CONST.AD.Groups.ServiceAdmin, False, session, notify_on_fail, notify_on_success)
+                return PIH.CHECK.ACCESS.by_group(AD.Groups.ServiceAdmin, False, session, notify_on_fail, notify_on_success)
 
             @staticmethod
             def inventory(session: SessionBase = None, notify_on_fail: bool = True, notify_on_success: bool = True) -> bool:
-                return PIH.CHECK.ACCESS.by_group(CONST.AD.Groups.Inventory, False, session, notify_on_fail, notify_on_success)
+                return PIH.CHECK.ACCESS.by_group(AD.Groups.Inventory, False, session, notify_on_fail, notify_on_success)
 
             @staticmethod
             def polibase(session: SessionBase = None, notify_on_fail: bool = True, notify_on_success: bool = True) -> bool:
-                return PIH.CHECK.ACCESS.by_group(CONST.AD.Groups.Polibase, False, session, notify_on_fail, notify_on_success)
+                return PIH.CHECK.ACCESS.by_group(AD.Groups.Polibase, False, session, notify_on_fail, notify_on_success)
 
             @staticmethod
             def card_registry(session: SessionBase = None, notify_on_fail: bool = True, notify_on_success: bool = True) -> bool:
-                return PIH.CHECK.ACCESS.by_group(CONST.AD.Groups.CardRegistry, False, session, notify_on_fail, notify_on_success)
+                return PIH.CHECK.ACCESS.by_group(AD.Groups.CardRegistry, False, session, notify_on_fail, notify_on_success)
 
         class USER:
 
             @staticmethod
+            def by_group(user: User, group: AD.Groups) -> bool:
+                return not DataTool.is_empty(ResultTool.do_while(PIH.RESULT.USER.by_group(group), lambda check_user: check_user.samAccountName == user.samAccountName))
+
+            @staticmethod
             def exists_by_login(value: str) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_user_exists_by_login, value))
 
             @staticmethod
             def user(user: User) -> bool:
                 return PIH.CHECK.full_name(user.name)
 
             @staticmethod
             def active(user: User) -> bool:
-                return user.distinguishedName.find(CONST.AD.ACTIVE_USERS_CONTAINER_DN) != -1
+                return user.distinguishedName.find(AD.ACTIVE_USERS_CONTAINER_DN) != -1
 
             @staticmethod
             def exists_by_full_name(full_name: FullName) -> bool:
                 return not ResultTool.is_empty(PIH.RESULT.USER.by_full_name(full_name))
 
             @staticmethod
             def search_attribute(value: str) -> bool:
-                return value in CONST.AD.SEARCH_ATTRIBUTES
+                return value in AD.SEARCH_ATTRIBUTES
 
             @staticmethod
-            def property(value: str, default_value: str = USER_PROPERTY.PASSWORD) -> str:
+            def property(value: str | None, default_value: str = USER_PROPERTY.PASSWORD) -> str:
                 return value or default_value
 
             @staticmethod
             def accessibility() -> bool:
                 return PIH.SERVICE.check_accessibility(ServiceRoles.AD)
 
         class MESSAGE:
@@ -3071,38 +3428,38 @@
 
                     @staticmethod
                     def accessibility(profile: Any, cached: bool = True) -> bool:
                         def internal_accessibility(profile: Any = None) -> bool:
                             profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                             url: str = f"{CONST.MESSAGE.WHATSAPP.WAPPI.URL_GET_STATUS}{profile}"
                             headers: dict = {
-                                "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORICATION,
+                                "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION,
                                 "Content-Type": "application/json"
                             }
                             response_result: dict = None
                             try:
                                 response: Response = requests.get(url, headers=headers)
                                 response_result = json.loads(response.text)
                             except Exception:
                                 return False
                             if "status" in response_result:
                                 if response_result["status"] == "error":
                                     return False
                             return response_result["app_status"] == "open"
-                        return PIH.CHECK.RESOURCE_MANAGER.wappi_profile_accessibility(profile, True) if cached else internal_accessibility(profile)
+                        return PIH.CHECK.RESOURCE.wappi_profile_accessibility(profile, True) if cached else internal_accessibility(profile)
 
         class MARK:
 
             @staticmethod
             def free(tab_number: str) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_mark_free, tab_number))
 
             @staticmethod
             def exists_by_full_name(full_name: FullName) -> bool:
-                result: Result[List[Mark]] = PIH.RESULT.MARK.by_name(
+                result: Result[list[Mark]] = PIH.RESULT.MARK.by_name(
                     FullNameTool.to_string(full_name))
                 return ResultTool.is_empty(result)
 
             @staticmethod
             def accessibility() -> bool:
                 return PIH.SERVICE.check_accessibility(ServiceRoles.MARK)
 
@@ -3110,15 +3467,15 @@
             def tab_number(value: str) -> bool:
                 return value.isdecimal()
 
         class TIME_TRACKING:
 
             @staticmethod
             def accessibility() -> bool:
-                return PIH.CHECK.ACCESS.by_group(CONST.AD.Groups.TimeTrackingReport)
+                return PIH.CHECK.ACCESS.by_group(AD.Groups.TimeTrackingReport)
 
         class INVENTORY:
 
             @staticmethod
             def is_report_file(file_path: str) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_inventory_report, file_path))
 
@@ -3156,61 +3513,66 @@
                 class CONFIRMATION:
 
                     @staticmethod
                     def exists(recipient: str, sender: str, state: int = None) -> bool:
                         result: Result[PolibasePersonNotificationConfirmation] = PIH.RESULT.POLIBASE.NOTIFICATION.CONFIRMATION.by(
                             recipient, sender)
                         return not ResultTool.is_empty(result) and (True if state is None else result.data.status == state)
+            
+            class DATABASE:
+
+                def creation_start_time(value: datetime) -> bool:
+                    return DateTimeTool.is_equal_by_time(value, PIH.SETTINGS.to_datetime(SETTINGS.POLIBASE_CREATION_DB_DUMP_START_TIME))
 
         @staticmethod
         def login(value: str) -> bool:
             pattern: str = r"^[a-z]+[a-z_0-9]{"+str(CONST.NAME_POLICY.PART_ITEM_MIN_LENGTH - 1) + ",}"
             return re.fullmatch(pattern, value, re.IGNORECASE) is not None
 
         class WORKSTATION:
 
             @staticmethod
             def name(value: str) -> bool:
                 value = PIH.DATA.FORMAT.string(value)
-                for prefix in CONST.AD.WORKSTATION_PREFIX_LIST:
+                for prefix in AD.WORKSTATION_PREFIX_LIST:
                     if value.startswith(prefix):
                         return True
                 return False
 
             @staticmethod
             def exists(name: str) -> bool:
                 return not ResultTool.is_empty(ResultTool.filter(PIH.RESULT.WORKSTATION.all_description(), lambda workstation: name.lower() == workstation.name.lower()))
 
             @staticmethod
-            def has_property(workstation: WorkstationDescription, property: CONST.AD.WSProperies) -> bool:
+            def has_property(workstation: WorkstationDescription, property: AD.WSProperies) -> bool:
                 return BM.has(workstation.properties, property)
 
             @staticmethod
             def watchable(workstation: WorkstationDescription) -> bool:
-                return PIH.CHECK.WORKSTATION.has_property(workstation, CONST.AD.WSProperies.Watchable)
+                return PIH.CHECK.WORKSTATION.has_property(workstation, AD.WSProperies.Watchable)
 
             @staticmethod
             def shutdownable(workstation: WorkstationDescription) -> bool:
-                return PIH.CHECK.WORKSTATION.has_property(workstation, CONST.AD.WSProperies.Shutdownable)
+                return PIH.CHECK.WORKSTATION.has_property(workstation, AD.WSProperies.Shutdownable)
 
             @staticmethod
             def rebootable(workstation: WorkstationDescription) -> bool:
-                return PIH.CHECK.WORKSTATION.has_property(workstation, CONST.AD.WSProperies.Rebootable)
+                return PIH.CHECK.WORKSTATION.has_property(workstation, AD.WSProperies.Rebootable)
 
         @staticmethod
         def telephone_number(value: str, international: bool = False) -> bool:
             return not DataTool.is_empty(value) and re.fullmatch(("" if international else r"^\+") + "[0-9]{11,13}$", value) is not None
 
         @staticmethod
         def telephone_number_international(value: str) -> bool:
             return PIH.CHECK.telephone_number(value, True)
 
         @staticmethod
         def email(value: str, check_accesability: bool = False) -> bool:
-            return re.fullmatch(r"([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\.[A-Z|a-z]{2,})+", value) is not None and (not check_accesability or PIH.CHECK.email_accessability(value))
+            return re.fullmatch(r"([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\.[A-Z|a-z]{2,})+", value) is not None and (not check_accesability or PIH.CHECK.EMAIL.accessability(value))
 
         @staticmethod
         def name(value: str, use_space: bool = False) -> bool:
             pattern = r"[а-яА-ЯёЁ" + (" " if use_space else "") + \
                 "]{" + str(CONST.NAME_POLICY.PART_ITEM_MIN_LENGTH) + ",}$"
             return re.fullmatch(pattern, value) is not None
 
@@ -3221,29 +3583,23 @@
             return re.fullmatch(pattern, value) is not None
 
         @staticmethod
         def password(value: str, settings: PasswordSettings = None) -> bool:
             settings = settings or PASSWORD.SETTINGS.DEFAULT
             return PasswordTools.check_password(value, settings.length, settings.special_characters)
 
-        @staticmethod
-        def ping(host: str) -> bool:
-            command = ['ping', "-n", '1', host]
-            response = subprocess.call(command)
-            return response == 0
-
 
     class LOG:
 
         executor = ThreadPoolExecutor(max_workers=1)
 
         @staticmethod
-        def send_message(value: str, channel: LogChannels = LogChannels.DEFAULT, level: Any = LogLevels.DEFAULT) -> None:
+        def send_message(value: str, channel: LogChannels = LogChannels.DEFAULT, level: Any = LogLevels.DEFAULT) -> str:
             level_value: int = None
-            level_list: List[LogLevels] = None
+            level_list: list[LogLevels] = None
             if isinstance(level, LogLevels):
                 level_list = [level]
             if isinstance(level, int):
                 level_value = level
             if level_value is None:
                 level_value = 0
                 for level_item in level_list:
@@ -3253,19 +3609,20 @@
                 try:
                     RPC.call(ServiceCommands.send_log_message,
                             (message, channel_name, level_value))
                 except Error as error:
                     PIH.output.error("Log send error")
             PIH.LOG.executor.submit(internal_send_message, value,
                                         channel.name, level_value)
+            return value
 
         @staticmethod
         def send_command(value: LogCommands, parameters: Tuple = None) -> None:
             message_commnad_description: LogCommandDescription = value.value
-            parameter_pattern_list: List = DataTool.as_list(
+            parameter_pattern_list: list = DataTool.as_list(
                 message_commnad_description.params)
             parameters = parameters or ()
             parameters_dict: dict = {}
             if len(parameter_pattern_list) > len(parameters):
                 raise Exception(
                     "Income parameter list length is less that parameter list length of command")
             for index, parameter_pattern_item in enumerate(parameter_pattern_list):
@@ -3282,105 +3639,136 @@
                                         value.name, parameters_dict)
 
         class COMMAND:
 
             @staticmethod
             def send(value: LogCommands, parameters: Tuple = None) -> None:
                 PIH.LOG.send_command(value, parameters)
+
+
+            @staticmethod
+            def computer_was_started(name: str) -> None:
+                PIH.LOG.send_command(
+                    LogCommands.COMPUTER_WAS_STARTED, (name,))
+                
+            @staticmethod
+            def server_was_started(name: str) -> None:
+                PIH.LOG.send_command(
+                    LogCommands.SERVER_WAS_STARTED, (name,))
     
             @staticmethod
-            def polibase_persons_with_old_format_barcode_was_detected(persons_pin: List[int]) -> None:
+            def polibase_persons_with_old_format_barcode_was_detected(persons_pin: list[int]) -> None:
                 PIH.LOG.send_command(
                     LogCommands.POLIBASE_PERSONS_WITH_OLD_FORMAT_BARCODE_WAS_DETECTED, (len(persons_pin), persons_pin))
 
             @staticmethod
-            def all_polibase_persons_barcode_with_old_format_was_created(persons_pin: List[int]) -> None:
+            def all_polibase_persons_barcode_with_old_format_was_created(persons_pin: list[int]) -> None:
                 PIH.LOG.send_command(
                     LogCommands.POLIBASE_ALL_PERSON_BARCODES_WITH_OLD_FORMAT_WAS_CREATED, (persons_pin,))
 
             @staticmethod
             def polibase_person_visit_was_registered(value: PolibasePersonVisitDS) -> None:
                 PIH.LOG.send_command(LogCommands.POLIBASE_PERSON_VISIT_WAS_REGISTERED, (
                     value.FullName, "Предзапись" if value.pin == CONST.POLIBASE.PRERECORDING_PIN else value.pin, value))
+                
+            @staticmethod
+            def resource_accessible(resource: ResourceStatus, at_first_time: bool) -> None:
+                PIH.LOG.send_command(LogCommands.RESOURCE_ACCESSABLE, (resource.name, resource, at_first_time))
+
+            @staticmethod
+            def resource_inaccessible(resource: ResourceStatus, at_first_time: bool, reason: RESOURCE.INACCESSABLE_REASON | None = None) -> None:
+                reason_string: str = ""
+                reason_name: str | None = None
+                if not DataTool.is_empty(reason):
+                    reason_string = f"Причина: {reason.value}"
+                    reason_name =  reason.name
+                PIH.LOG.send_command(LogCommands.RESOURCE_INACCESSABLE, (resource.name, resource, at_first_time, reason_string, reason_name))
 
             @staticmethod
             def polibase_person_visit_notification_was_registered(visit: PolibasePersonVisitDS, notification: PolibasePersonVisitNotificationDS) -> None:
                 PIH.LOG.send_command(LogCommands.POLIBASE_PERSON_VISIT_NOTIFICATION_WAS_REGISTERED, (
                     visit.FullName, "Предзапись" if visit.pin == CONST.POLIBASE.PRERECORDING_PIN else visit.pin, notification))
 
             @staticmethod
             def login() -> None:
                 login: str = PIH.session.get_login()
                 user: User = PIH.RESULT.USER.by_login(login).data
                 PIH.LOG.send_command(
-                    LogCommands.LOG_IN, (user.name, login, PIH.OS.get_host()))
+                    LogCommands.LOG_IN, (user.name, login, PIH.OS.host()))
 
             @staticmethod
             def whatsapp_message_received(message: WhatsAppMessage) -> None:
                 PIH.LOG.send_command(
                     LogCommands.WHATSAPP_MESSAGE_RECEIVED, (message,))
 
             @staticmethod
+            def new_file_detected(path: str) -> None:
+                PIH.LOG.send_command(
+                    LogCommands.NEW_FILE_DETECTED, (path,))
+                
+            @staticmethod
+            def new_polibase_scanned_document_detected(value: PolibaseScannedDocument):
+                PIH.LOG.send_command(LogCommands.NEW_POLIBASE_DOCUMENT_DETECTED, (value.file_path, value.pin, value.document_name))
+
+            @staticmethod
             def start_session() -> None:
-                argv: List[str] = PIH.session.argv
+                argv: list[str] = PIH.session.argv
                 argv_str: str = ""
                 if not DataTool.is_empty(argv):
                     argv_str = " ".join(argv)
                     argv_str = f"({argv_str})"
                 login: str = PIH.session.get_login()
                 user: User = PIH.RESULT.USER.by_login(login).data
                 PIH.LOG.send_command(LogCommands.SESSION_STARTED, (user.name, login,
-                                         f"{PIH.session.file_name} {argv_str}", f"{PIH.VERSION.local()}/{PIH.VERSION.remote()}", PIH.OS.get_host()))
+                                         f"{PIH.session.file_name} {argv_str}", f"{PIH.VERSION.local()}/{PIH.VERSION.remote()}", PIH.OS.host()))
 
             @staticmethod
             def backup_notify_about_robocopy_job_started(status: str) -> None:
                 PIH.LOG.send_command(
                     LogCommands.BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_STARTED, (status, ))
 
             @staticmethod
             def backup_notify_about_robocopy_job_completed(status: str) -> None:
                 PIH.LOG.send_command(
                     LogCommands.BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_COMPLETED, (status, ))
 
             @staticmethod
-            def service_action(role: ServiceRoles, log_command: LogCommands) -> None:
-                service_role_value: ServiceRoleDescription = role.value
-                PIH.LOG.send_command(log_command, (role.name, service_role_value.description,
-                                         service_role_value.host, service_role_value.port, service_role_value.pid))
+            def service_action(service_role_description: ServiceRoleDescription, log_command: LogCommands) -> None:
+                PIH.LOG.send_command(log_command, (service_role_description.name, service_role_description.description,
+                                         service_role_description.host, service_role_description.port, service_role_description.pid))
 
             @staticmethod
-            def service_started(role: ServiceRoles) -> None:
-                PIH.LOG.COMMAND.service_action(role, LogCommands.SERVICE_STARTED)
+            def service_started(service_role_description: ServiceRoleDescription) -> None:
+                PIH.LOG.COMMAND.service_action(service_role_description, LogCommands.SERVICE_STARTED)
             
             @staticmethod
-            def service_starts(role: ServiceRoles) -> None:
-                PIH.LOG.COMMAND.service_action(role, LogCommands.SERVICE_STARTS)
+            def service_starts(service_role_description: ServiceRoleDescription) -> None:
+                PIH.LOG.COMMAND.service_action(service_role_description, LogCommands.SERVICE_STARTS)
 
             @staticmethod
-            def service_is_inaccessable_and_waiting_to_be_restarted(role: ServiceRoles) -> None:
-                PIH.LOG.COMMAND.service_action(role, LogCommands.SERVICE_IS_INACCESIBLE_AND_WAITING_TO_BE_RESTARTED)
+            def service_is_inaccessable_and_waiting_to_be_restarted(service_role_description: ServiceRoleDescription) -> None:
+                PIH.LOG.COMMAND.service_action(service_role_description, LogCommands.SERVICE_IS_INACCESIBLE_AND_WAITING_TO_BE_RESTARTED)
 
             @staticmethod
-            def service_not_started(role: ServiceRoles, error: str) -> None:
-                service_role_value: ServiceRoleDescription = role.value
-                PIH.LOG.send_command(LogCommands.SERVICE_NOT_STARTED, (role.name, service_role_value.description,
-                                         service_role_value.host, service_role_value.port, error))
+            def service_not_started(service_role_description: ServiceRoleDescription, error: str) -> None:
+                PIH.LOG.send_command(LogCommands.SERVICE_NOT_STARTED, (service_role_description.name, service_role_description.description,
+                                                                       service_role_description.host, service_role_description.port, error))
 
             @staticmethod
             def hr_notify_about_new_employee(login: User) -> None:
                 user: User = PIH.RESULT.USER.by_login(login).data
                 hr_user: User = ResultTool.get_first_element(
-                    PIH.RESULT.USER.by_job_position(CONST.AD.JobPisitions.HR))
+                    PIH.RESULT.USER.by_job_position(AD.JobPisitions.HR))
                 PIH.LOG.send_command(LogCommands.HR_NOTIFY_ABOUT_NEW_EMPLOYEE, (FullNameTool.to_given_name(hr_user.name),
                                                                                         user.name, user.mail))
 
             @staticmethod
             def it_notify_about_user_creation(login: str, password: str) -> None:
-                it_user_list: List[User] = PIH.RESULT.USER.by_job_position(
-                    CONST.AD.JobPisitions.IT).data
+                it_user_list: list[User] = PIH.RESULT.USER.by_job_position(
+                    AD.JobPisitions.IT).data
                 me_user_login: str = PIH.session.get_login()
                 it_user_list = list(
                     filter(lambda user: user.samAccountName != me_user_login, it_user_list))
                 it_user: User = it_user_list[0]
                 user: User = PIH.RESULT.USER.by_login(login).data
                 PIH.LOG.send_command(LogCommands.IT_NOTIFY_ABOUT_CREATE_USER, (
                     user.name, user.description, user.samAccountName, password, user.telephoneNumber, user.mail))
@@ -3462,175 +3850,200 @@
                     True, full_name, tab_number)
 
             @staticmethod
             def printer_report(name: str, location: str, report: str) -> bool:
                 return PIH.LOG.send_command(LogCommands.PRINTER_REPORT, (name, location, report))
 
         @staticmethod
-        def to_debug_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def debug_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.DEBUG_BOT, level)
 
         @staticmethod
-        def from_debug_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def debug(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.DEBUG, level)
 
         @staticmethod
-        def from_service_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def services(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.SERVICE, level)
 
         @staticmethod
-        def from_resources_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def resources(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.RESOURCES, level)
         
         @staticmethod
-        def from_printer_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def printers(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.PRINTER, level)
 
         @staticmethod
-        def to_service_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def services_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.SERVICE_BOT, level)
 
         @staticmethod
-        def backup(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def backup(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.BACKUP, level)
 
         @staticmethod
-        def from_notification_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def notification(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.NOTIFICATION, level)
 
         @staticmethod
-        def to_notification_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def notification_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.NOTIFICATION_BOT, level)
 
         @staticmethod
-        def from_it_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def it(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.IT, level)
 
         @staticmethod
-        def from_feedback_call_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def from_feedback_call_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.POLIBASE_PERSON_FEEDBACK_CALL, level)
 
         @staticmethod
-        def from_review_request_result(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def from_review_request_result(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.POLIBASE_PERSON_REVIEW_QUEST_RESULT, level)
 
         @staticmethod
-        def to_it_bot(message: str, level: Any = LogLevels.DEFAULT) -> Any:
+        def it_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
             return PIH.LOG.send_message(message, LogChannels.IT_BOT, level)
 
 
     class MESSAGE:
 
         class POLIBASE:
 
-            class ADMIN:
+            @staticmethod
+            def notify(message: str, test: bool = True) -> None:
+                PIH.MESSAGE.WORKSTATION.to_all_workstations(message, AD.Groups.PolibaseUsers, [CONST.HOST.WS255.NAME], None, test, 180)
+
+            @staticmethod
+            def notify_about_polibase_closing(message: str | None = None, test: bool = True) -> None:
+                PIH.MESSAGE.POLIBASE.notify(message or PIH.SETTINGS.get(
+                    SETTINGS.POLIBASE_WAS_EMERGENCY_CLOSED_NOTIFICATION_TEXT), test)
+                
+            @staticmethod
+            def notify_about_polibase_restarted(test: bool = True) -> None:
+                PIH.MESSAGE.POLIBASE.notify(PIH.SETTINGS.get(
+                    SETTINGS.POLIBASE_WAS_RESTARTED_NOTIFICATION_TEXT), test)
 
-                @staticmethod
-                def notify_about_polibase_emergency_closing(test: bool = True) -> None:
-                    PIH.MESSAGE.WORKSTATION.to_all_workstations(PIH.SETTINGS.get(
-                        SETTINGS.POLIBASE_WAS_EMERGENCY_CLOSED_NOTIFICATION_TEXT), CONST.AD.Groups.PolibaseUsers, [CONST.HOST.WS255.NAME], None, test)
 
         class WORKSTATION:
               
             executor = ThreadPoolExecutor(max_workers=10)
 
             @staticmethod
-            def to_all_workstations(message: str, filter_group: CONST.AD.Groups = None, to_all_user_workstation_name_list: List[str] = None, session: Session = None, test: bool = True) -> None:
+            def to_all_workstations(message: str, filter_group: AD.Groups = None, to_all_user_workstation_name_list: list[str] = None, session: Session = None, test: bool = True, timeout: int = 60) -> None:
                 session = session or PIH.session
-                filter_user_login_list: List[str] = None if filter_group is None else ResultTool.map(PIH.RESULT.USER.by_group(filter_group), lambda item: item.samAccountName).data
+                filter_user_login_list: list[str] = None if filter_group is None else ResultTool.map(PIH.RESULT.USER.by_group(filter_group), lambda item: item.samAccountName.lower()).data
                 filter_user_login_list_is_empty: bool = DataTool.is_empty(filter_user_login_list)
                 to_all_user_workstation_name_list_is_empty: bool = DataTool.is_empty(
                     to_all_user_workstation_name_list)
                 def filter_function(workstation: Workstation) -> bool:
-                    return workstation.accessable and ((filter_user_login_list_is_empty or workstation.samAccountName in filter_user_login_list) or (to_all_user_workstation_name_list_is_empty or workstation.name.lower() in to_all_user_workstation_name_list))
+                    workstation_name: str = workstation.name.lower()
+                    if test:
+                        return workstation_name == CONST.TEST.WS
+                    return workstation.accessable and ((filter_user_login_list_is_empty or workstation.samAccountName in filter_user_login_list) or (to_all_user_workstation_name_list_is_empty or workstation_name in to_all_user_workstation_name_list))
                 def every_action(workstation: Workstation) -> None:
-                    def internal_send_message(user_login: str, workstation_name: str, message: str) -> None:
+                    def internal_send_message(user_login: str | None, workstation_name: str, message: str) -> None:
                         if not DataTool.is_empty(to_all_user_workstation_name_list) and workstation_name in to_all_user_workstation_name_list:
                             if not test:
-                                PIH.MESSAGE.WORKSTATION.to_user_or_workstation(None, workstation_name, message)
+                                PIH.MESSAGE.WORKSTATION.to_user_or_workstation(None, workstation_name, message, timeout)
                         else:
                             if DataTool.is_empty(user_login):
-                                pass
+                                if test:
+                                    PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message, timeout)
+                                else:
+                                    pass
                                 #dont send message - cause workstation is on but no one user is logged
                             else:
                                 if test:
                                     if workstation_name == CONST.TEST.WS:
-                                        PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message)
+                                        PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message, timeout)
                                 else:
-                                    PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message)
+                                    PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message, timeout)
                     result_message: str = f"Сообщение от {session.user_given_name} ({A.D_F.description(session.get_user().description)}):"
                     result_message += f" День добрый, "
                     user_data: dict = {"user" : None}
                     def obtain_user_action() -> User:
                         user: User = None
                         try:
                             user = A.R_U.by_login(workstation.samAccountName).data
                             user_data["user"] = user
                         except NotFound:
                             pass
                         return user
                     if workstation.samAccountName:
                         while_not_do(lambda: obtain_user_action() is not None)
-                    user: User = user_data["user"]
-                    result_message += ("" if workstation.samAccountName is None else FullNameTool.to_given_name(user)) + ", "
+                    user: User | None = user_data["user"]
+                    result_message += "" if A.D_C.empty(workstation.samAccountName) else f"{FullNameTool.to_given_name(user)}, "
                     result_message += message
                     PIH.MESSAGE.WORKSTATION.executor.submit(
                         internal_send_message, workstation.samAccountName, workstation.name.lower(), result_message)
                 ResultTool.every(ResultTool.filter(PIH.RESULT.WORKSTATION.all(), filter_function), every_action)
 
             @staticmethod
-            def to_user(value: Any, message: str, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
-                return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(value.samAccountName if isinstance(value, User) else value, None, message, method_type)
+            def to_user(value: Any, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
+                return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(value.samAccountName if isinstance(value, User) else value, None, message, timeout, method_type)
 
             @staticmethod
-            def to_workstation(value: Any, message: str, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
-                return PIH.MESSAGE.WORKSTATION.by_workstation_name(value.name if isinstance(value, WorkstationDescription) else value, message, method_type)
+            def to_workstation(value: Any, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
+                return PIH.MESSAGE.WORKSTATION.by_workstation_name(value.name if isinstance(value, WorkstationDescription) else value, message, timeout, method_type)
 
             @staticmethod
-            def by_workstation_name(value: str, message: str, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
+            def by_workstation_name(value: str, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
                 user: User = None
                 try:
                     user = PIH.RESULT.USER.by_workstation_name(value).data
                 except NotFound:
                     pass
-                return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user.samAccountName if user is not None else None, value, message, method_type)
+                return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user.samAccountName if user is not None else None, value, message, timeout, method_type)
 
             @staticmethod
-            def to_user_or_workstation(user_login: str, workstation_name: str, message: str, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
-                if RPC.Service.role == ServiceRoles.WS:
+            def to_user_or_workstation(user_login: str, workstation_name: str, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
+                if RPC.Service.role_description is not None and RPC.Service.role_description.name == ServiceRoles.WS.value.name:
                     method_type = WorkstationMessageMethodTypes.LOCAL_PSTOOL_MSG
                 if method_type == WorkstationMessageMethodTypes.REMOTE:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.send_message_to_user_or_workstation, (user_login, workstation_name, message)))
+                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.send_message_to_user_or_workstation, (user_login, workstation_name, message, timeout)))
                 def internal_send_by_login_and_workstation_name(login: str, workstation_name: str) -> None:
                     if method_type == WorkstationMessageMethodTypes.LOCAL_PSTOOL_MSG:
                         PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
-                            [CONST.MSG.EXECUTOR, login, message], workstation_name), False)
+                            [CONST.MSG.EXECUTOR, f"/time:{timeout}", login, message], workstation_name), False)
                     if method_type == WorkstationMessageMethodTypes.LOCAL_MSG:
                         PIH.PSTOOLS.execute_command_list(
-                            [CONST.MSG.EXECUTOR, login, f"/server:{workstation_name}", message], False)
+                            [CONST.MSG.EXECUTOR, f"/time:{timeout}", login, f"/server:{workstation_name}", message], False)
                 if workstation_name is None:
                     ResultTool.every(PIH.RESULT.WORKSTATION.by_login(
                         user_login), lambda workstation: internal_send_by_login_and_workstation_name(user_login, workstation.name))
                 else:
                     if user_login is None:
                         internal_send_by_login_and_workstation_name(
                             "*", workstation_name)
                     else:
                         internal_send_by_login_and_workstation_name(
                             user_login, workstation_name)
                 return True
 
             @staticmethod
-            def by_login(login: str, message: str, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
-                return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(login, None, message, method_type)
+            def by_login(login: str, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
+                return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(login, None, message, timeout, method_type)
 
         class WHATSAPP:
 
             class WAPPI:
 
+                class QUEUE:
+    
+                    @staticmethod
+                    def add(message: Message, recipient: str, sender: CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE, high_priority: bool = False) -> bool:
+                        return PIH.MESSAGE.WHATSAPP.WAPPI.QUEUE.add_message(Message(message, recipient, sender.value), high_priority)
+                    
+                    @staticmethod
+                    def add_message(message: Message, high_priority: bool = False) -> bool:
+                        return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.add_message_to_queue, (message, high_priority)))
+
+
                 WAPPI_PROFILE_MAP: dict = None 
 
                 @staticmethod
                 def get_wappi_collection() -> dict:
                     WP = CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE
                     result: dict = PIH.MESSAGE.WHATSAPP.WAPPI.WAPPI_PROFILE_MAP or {
                         WP.IT: PIH.DATA.TELEPHONE_NUMBER.it_administrator(),
@@ -3653,22 +4066,22 @@
                     profile_id_collection = PIH.MESSAGE.WHATSAPP.WAPPI.get_wappi_collection()
                     for item in profile_id_collection:
                         if profile_id_collection[item] == telephone_number:
                             return item
                     return None
 
                 @staticmethod
-                def get_message_list(telephone_number: str, profile: Any = None) -> List[WhatsAppMessage]:
+                def get_message_list(telephone_number: str, profile: Any = None) -> list[WhatsAppMessage]:
                     profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                     url: str = f"{CONST.MESSAGE.WHATSAPP.WAPPI.URL_GET_MESSAGES}{profile}&chat_id={telephone_number}{CONST.MESSAGE.WHATSAPP.WAPPI.CONTACT_SUFFIX}"
                     headers: dict = {
-                        "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORICATION,
+                        "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION,
                         "Content-Type": "application/json"
                     }
-                    result: List[WhatsAppMessage] = []
+                    result: list[WhatsAppMessage] = []
                     try:
                         response: Response = requests.get(url, headers=headers)
                     except Exception:
                         return result
                     response_result: dict = json.loads(response.text)
                     has_error: bool = response_result["status"] == "error" or ("detail" in response_result and response_result["detail"] == "Messages not found")
                     if not has_error:
@@ -3676,14 +4089,15 @@
                             if message_item["type"] == "chat":
                                 result.append(WhatsAppMessage(message_item["body"], message_item["fromMe"], str(message_item["from"]).split("@")[0], 
                                    str(message_item["to"]).split("@")[0], profile, message_item["time"]))
                     return result 
                 
                 @staticmethod
                 def send(telephone_number: str, message: Any, profile: Any = None) -> bool:
+                    #print(message)
                     profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                     url: str = None
                     payload: dict = {"recipient": telephone_number}
                     if isinstance(message, str):
                         payload["body"] = message
                         url: str = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_MESSAGE
                     elif isinstance(message, (WhatsAppMessageListPayload, WhatsAppMessageButtonsPayload)):
@@ -3693,67 +4107,66 @@
                                 payload[item] = item_value
                         if isinstance(message, WhatsAppMessageListPayload):
                             url = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_LIST_MESSAGE
                         else:
                             url = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_BUTTONS_MESSAGE
                     url += profile
                     headers: dict = {"accept": "application/json",
-                                     "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORICATION, "Content-Type": "application/json"}
+                                     "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION, "Content-Type": "application/json"}
                     try:
                         response: Response = requests.post(
                             url, data=json.dumps(payload), headers=headers)
                     except ConnectTimeout:
+                        #print("ConnectTimeout")
                         return False
                     if response.status_code == CONST.ERROR.WAPPI.PROFILE_NOT_PAID:
-                        PIH.LOG.from_resources_bot(
+                        PIH.LOG.resources(
                             "Аккаунт Wappi (сервис для отправики сообщений в WhatsApp) не оплачен", LogLevels.ERROR)
                     status_code: int = response.status_code
+                    #print(status_code)
                     return status_code == 200
 
                 @staticmethod
-                def send_video(telephone_number: str, caption: str, base64_value: str,  profile: Any = None) -> bool:
+                def send_base64_file(url: str, telephone_number: str, caption: str, base64_content: str,  profile: Any = None) -> bool:
                     profile = EnumTool.get_value(
                         profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                     payload: dict = {"recipient": telephone_number,
                                      "caption": caption,
-                                     "b64_file": base64_value}
+                                     "b64_file": base64_content}
                     headers: dict = {"accept": "application/json",
-                                     "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORICATION, "Content-Type": "application/json"}
-                    url: str = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_VIDEO + profile
+                                     "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION, "Content-Type": "application/json"}
+                    url = url + profile
                     try:
                         response: Response = requests.post(
                             url, data=json.dumps(payload), headers=headers)
                     except ConnectTimeout:
                         return False
                     if response.status_code == CONST.ERROR.WAPPI.PROFILE_NOT_PAID:
-                        PIH.LOG.from_resources_bot(
+                        PIH.LOG.resources(
                             "Аккаунт Wappi (сервис для отправики сообщений в WhatsApp) не оплачен", LogLevels.ERROR)
                     return response.status_code == 200
 
                 @staticmethod
-                def send_image(telephone_number: str, caption: str, base64_value: str, profile: Any = None) -> bool:
-                    profile = EnumTool.get_value(
-                        profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
-                    payload: dict = {"recipient": telephone_number,
-                                     "caption": caption,
-                                     "b64_file": base64_value}
-                    headers: dict = {"accept": "application/json",
-                                     "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORICATION, "Content-Type": "application/json"}
-                    url: str = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_IMAGE + profile
-                    try:
-                        response: Response = requests.post(
-                            url, data=json.dumps(payload), headers=headers)
-                    except ConnectTimeout:
-                        return False
-                    if response.status_code == CONST.ERROR.WAPPI.PROFILE_NOT_PAID:
-                        PIH.LOG.from_resources_bot(
-                            "Аккаунт Wappi (сервис для отправики сообщений в WhatsApp) не оплачен", LogLevels.ERROR)
-                    return response.status_code == 200
+                def send_video(telephone_number: str, caption: str, base64_content: str, profile: Any = None) -> bool:
+                    return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_VIDEO, telephone_number, caption, base64_content, profile)
+
+                @staticmethod
+                def send_image(telephone_number: str, caption: str, base64_content: str, profile: Any = None) -> bool:
+                    return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_IMAGE, telephone_number, caption, base64_content, profile)
+
+                @staticmethod
+                def send_document(telephone_number: str, caption: str, base64_content: str, profile: Any = None) -> bool:
+                    return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_DOCUMENT, telephone_number, caption, base64_content, profile)
 
             @staticmethod
+            def create_output(recipient: str) -> Output:
+                from MobileHelperCore.api import WappiOutput, WappiSession
+                return WappiOutput(WappiSession(recipient))
+            
+            @staticmethod
             def send_via_browser(telephone_number: str, message: str) -> bool:
                 pywhatkit_is_exists: bool = importlib.util.find_spec(
                     "pywhatkit") is not None
                 if not pywhatkit_is_exists:
                     PIH.output.green(
                         "Установка библиотеки для отправки сообщения. Ожидайте...")
                     if not PIH.UPDATER.install_module("pywhatkit"):
@@ -3791,32 +4204,60 @@
             @staticmethod
             def send_image(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any = None) -> bool:
                 wappi_profile = EnumTool.get_value(
                     wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                 telephone_number = PIH.DATA.FORMAT.telephone_number(
                     telephone_number)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_image(telephone_number, caption, base64_value, wappi_profile)
+        
+            @staticmethod
+            def send_document(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any = None) -> bool:
+                wappi_profile = EnumTool.get_value(
+                    wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
+                telephone_number = PIH.DATA.FORMAT.telephone_number(
+                    telephone_number)
+                return PIH.MESSAGE.WHATSAPP.WAPPI.send_document(telephone_number, caption, base64_value, wappi_profile)
 
             @staticmethod
             def send_to_user(user: User, message: Any, via_wappi: bool = True, use_alternative: bool = True, wappi_profile: Any = None) -> bool:
                 return PIH.MESSAGE.WHATSAPP.send(user.telephoneNumber, message, via_wappi, use_alternative, EnumTool.get_value(
                     wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value))
 
         class DELAYED:
 
             @staticmethod
             def register(message: DelayedMessage) -> int:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.register_delayed_message, PIH.ACTION.MESSAGE.DELAYED.prepeare_message(message)))
 
             @staticmethod
-            def send(message: DelayedMessage, register: bool = True, add_to_top: bool = True) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.send_delayed_message, (PIH.ACTION.MESSAGE.DELAYED.prepeare_message(message), register, add_to_top)))
+            def send(message: DelayedMessage, high_priority: bool = True) -> bool:
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.send_delayed_message, (PIH.ACTION.MESSAGE.DELAYED.prepeare_message(message), high_priority)))
+            
     
     class ACTION:
 
+        class QR_CODE:
+
+            @staticmethod
+            def titled(data: str, title, path: str, font_size: int | None = None) -> bool:
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_qr_code, (data, title, path, font_size)))
+
+            @staticmethod
+            def print(path: str) -> bool:
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.print_image, (path, )))
+
+            @staticmethod
+            def for_mobile_helper_command(value: str, title: str, path: str, font_size: int | None = None) -> bool:
+                return PIH.ACTION.QR_CODE.titled(PIH.DATA.FORMAT.mobile_helper_qr_code_text(PIH.DATA.FORMAT.mobile_helper_command(value)), title, path, font_size)
+            
+            @staticmethod
+            def for_polibase_person_card_registry_folder(name: str) -> bool:
+                name = A.D_F.polibase_person_card_registry_folder(name)
+                return PIH.ACTION.QR_CODE.for_mobile_helper_command(" ".join(["card", "registry", name]), name, PIH.PATH.QR_CODE.polibase_person_card_registry_folder(name), 80)
+
         class INDICATION:
 
             class CT:
 
                 @staticmethod
                 def register(value: CTIndicationValue) -> bool:
                     return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.register_ct_indications_value, (value), ))
@@ -3853,41 +4294,41 @@
             class DELAYED:
 
                 @staticmethod
                 def update(value: DelayedMessageDS, search_critery: MessageSearchCritery) -> bool:
                     return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.update_delayed_message, (value, search_critery)))
 
                 @staticmethod
-                def update_status(value: DelayedMessageDS, status: MessageStatus) -> bool:
+                def update_status(value: DelayedMessageDS, status: MessageStatuses) -> bool:
                     return PIH.ACTION.MESSAGE.DELAYED.update(DelayedMessageDS(status=status.value), MessageSearchCritery(id=value.id))
 
                 @staticmethod
                 def complete(value: DelayedMessageDS) -> bool:
-                    return PIH.ACTION.MESSAGE.DELAYED.update_status(value, MessageStatus.COMPLETE)
+                    return PIH.ACTION.MESSAGE.DELAYED.update_status(value, MessageStatuses.COMPLETE)
 
                 @staticmethod
                 def abort(value: DelayedMessageDS) -> bool:
-                    return PIH.ACTION.MESSAGE.DELAYED.update_status(value, MessageStatus.ABORT)
+                    return PIH.ACTION.MESSAGE.DELAYED.update_status(value, MessageStatuses.ABORT)
 
                 @staticmethod
                 def prepeare_message(message: DelayedMessage) -> DelayedMessage:
                     if message.type is None:
                         message.type = MessageTypes.WHATSAPP.value
                     if message.date is not None:
                         if isinstance(message.date, datetime):
-                            message.date = DateTimeTool.to_string(
+                            message.date = DateTimeTool.datetime_to_string(
                                 message.date, CONST.DATA_STORAGE.DATE_TIME_FORMAT)
                     if message.sender is not None:
                         message.sender = EnumTool.get_value(message.sender)
                     if  message.type == MessageTypes.WHATSAPP.value and not DataTool.is_empty(message.recipient):
                         if PIH.CHECK.telephone_number(message.recipient):
                             #+7 -> 7
                             message.recipient = PIH.DATA.FORMAT.telephone_number(message.recipient, CONST.INTERNATIONAL_TELEPHONE_NUMBER_PREFIX)
                     return message
-
+        
         class SETTINGS:
 
             @staticmethod
             def key(key: str, value: Any) -> bool:
                 return DataTool.rpc_unrepresent(
                     RPC.call(ServiceCommands.set_settings_value, (key, value)))
 
@@ -3926,29 +4367,26 @@
             @staticmethod
             def remove(user: User) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.remove_user, user.distinguishedName))
 
         class TIME_TRACKING:
 
             @staticmethod
-            def report(path: str, start_date: datetime, end_date: datetime, tab_number: str = None, plain_format: bool = False) -> bool:
-                now: datetime = datetime.now()
-                start_date = now.replace(hour=0, minute=0, day=start_date.day, second=0, month=start_date.month, year=start_date.year)
-                end_date = now.replace(hour=23, minute=59, second=0, day=end_date.day, month=end_date.month, year=end_date.year)
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_time_tracking_report, (path, start_date, end_date, tab_number, plain_format)))
+            def save_report(path: str, start_date: datetime, end_date: datetime, tab_number_list: list[str] = None, plain_format: bool = False) -> bool:
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.save_time_tracking_report, (path, DateTimeTool.start_date(start_date), DateTimeTool.end_date(end_date), tab_number_list, plain_format)))
 
         class INVENTORY:
 
             @staticmethod
             def create_barcodes(report_file_path: str, result_directory: str) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_barcodes_for_inventory, (report_file_path, result_directory)))
 
             @staticmethod
             def save_report_item(report_file_path: str, item: InventoryReportItem) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.save_report_item, (report_file_path, item)))
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.save_inventory_report_item, (report_file_path, item)))
 
             @staticmethod
             def close_report(report_file_path: str) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.close_inventory_report, report_file_path))
 
         class PRINTER:
 
@@ -3958,37 +4396,35 @@
 
             @staticmethod
             def status() -> bool:
                 return not ResultTool.is_empty(PIH.RESULT.PRINTER.status())
 
         class POLIBASE:
 
-            class ADMIN:
+            executor: ThreadPoolExecutor = ThreadPoolExecutor(max_workers=10)
 
-                executor: ThreadPoolExecutor = ThreadPoolExecutor(max_workers=10)
-
-                @staticmethod
-                def close_for_all(notify: bool = True, test: bool = True) -> None:
-                    def internal_close_action(workstation_name: str) -> None:
-                        PIH.ACTION.POLIBASE.ADMIN.close_by_workstation_name(workstation_name)
-                    def filter_function(workstation: Workstation) -> bool:
-                        return workstation.name == CONST.TEST.WS if test else workstation.accessable 
-                    def every_action(workstation: Workstation) -> None:
-                        PIH.ACTION.POLIBASE.ADMIN.executor.submit(internal_close_action, workstation.name.lower())
-                    if notify:
-                        PIH.MESSAGE.POLIBASE.ADMIN.notify_about_polibase_emergency_closing(test)
-                    ResultTool.every(ResultTool.filter(PIH.RESULT.WORKSTATION.all(), filter_function), every_action)
+            @staticmethod
+            def program_close_for_all(notify: bool = True, notification_message: str | None = None, test: bool = True) -> None:
+                def close_action(workstation: Workstation) -> None:
+                    PIH.ACTION.POLIBASE.client_program_close_for_workstation(workstation)
+                def filter_function(workstation: Workstation) -> bool:
+                    return workstation.name == CONST.TEST.WS if test else workstation.accessable 
+                def every_action(workstation: Workstation) -> None:
+                    PIH.ACTION.POLIBASE.executor.submit(close_action, workstation)
+                if notify:
+                    PIH.MESSAGE.POLIBASE.notify_about_polibase_closing(notification_message, test)
+                ResultTool.every(ResultTool.filter(PIH.RESULT.WORKSTATION.all(), filter_function), every_action)
 
-                @staticmethod
-                def close_by_workstation_name(value: str, test: bool = True) -> bool:
-                    return PIH.ACTION.WORKSTATION.kill_process(
-                        CONST.POLIBASE.PROCESS_NAME, value, test)
+            @staticmethod
+            def client_program_close_for_workstation(workstation: Workstation) -> bool:
+                return PIH.ACTION.WORKSTATION.kill_process(
+                    CONST.POLIBASE.PROCESS_NAME, workstation.name)
 
-            class SETTINGS:
-                pass
+            def restart(test: bool = True) -> None:
+                PIH.PSTOOLS.reboot(HOSTS.POLIBASE_TEST.NAME if test else HOSTS.POLIBASE.NAME)
 
             class NOTIFICATION:
 
                 @staticmethod
                 def register(value: PolibasePersonVisitNotificationDS) -> bool:
                     return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.register_polibase_person_visit_notification, value))
 
@@ -3999,32 +4435,32 @@
                         return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.update_polibase_person_notification_confirmation, PolibasePersonNotificationConfirmation(recepient, sender, status)))
 
             class INFORMATION_QUEST:
 
                 @staticmethod
                 def register(person: PolibasePerson) -> bool:
                     return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.register_polibase_person_information_quest, PolibasePersonInformationQuest(person.pin, person.FullName, person.telephoneNumber)))
+                
+                @staticmethod
+                def start(person: PolibasePerson) -> bool:
+                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.start_polibase_person_information_quest, (person.pin, )))
 
                 @staticmethod
                 def update(value: PolibasePersonInformationQuest, search_critery: PolibasePersonInformationQuest) -> bool:
                     return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.update_polibase_person_information_quest, (value, search_critery)))
 
             @staticmethod
             def create_barcode_for_person(pid: int, test: bool = None) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_barcode_for_polibase_person, (pid, test)))
 
             @staticmethod
             def set_card_folder_for_person(name: str, pid: int, test: bool = None) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_polibase_person_card_folder_name, (name, pid, test)))
 
             @staticmethod
-            def create_barcode_for_person_card_folder(value: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_barcode_for_polibase_person_card_registry_folder, (value, value)))
-
-            @staticmethod
             def set_email(value: str, pin: int, test: bool = None) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_polibase_person_email, (value, pin, test)))
 
             @staticmethod
             def set_person_barcode_by_pin(barcode_file_name: str, pin: int, test: bool = None) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_polibase_person_barcode_by_pin, (barcode_file_name, pin, test)))
 
@@ -4066,41 +4502,49 @@
 
             @staticmethod
             def remove(mark: Mark) -> bool:
                 return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.remove_mark_by_tab_number, mark.TabNumber))
 
         class DOCUMENTS:
 
+            @staticmethod 
+            def save_base64_as_image(path: str, content: str) -> bool:
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.save_base64_as_image, (path, content)))
+
             @staticmethod
             def create_for_user(path: str, full_name: FullName, tab_number: str, pc: LoginPasswordPair, polibase: LoginPasswordPair, email: LoginPasswordPair) -> bool:
                 locale.setlocale(locale.LC_ALL, 'ru_RU')
                 date_now = datetime.now().date()
                 date_now_string = f"{date_now.day} {calendar.month_name[date_now.month]} {date_now.year}"
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_user_document, (path, date_now_string, CONST.SITE_ADDRESS, CONST.SITE_PROTOCOL + CONST.SITE_ADDRESS, CONST.EMAIL_ADDRESS, full_name, tab_number, pc, polibase, email)))
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_user_document, (path, date_now_string, CONST.SITE_ADDRESS, CONST.SITE_PROTOCOL + CONST.SITE_ADDRESS, CONST.MAIL_ADDRESS, full_name, tab_number, pc, polibase, email)))
 
         class WORKSTATION:
     
             @staticmethod
-            def reboot(name: str = None, force: bool = False) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.reboot, (name, force)))
+            def reboot(host: str = None, force: bool = False) -> bool:
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.reboot, (host, force)))
 
             @staticmethod
-            def shutdown(name: str = None, force: bool = False) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.shutdown, (name, force)))
+            def shutdown(host: str = None, force: bool = False) -> bool:
+                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.shutdown, (host, force)))
             
             @staticmethod
-            def kill_process(process_name: str, workstation_name: str, test: bool = True) -> bool:
-                return PIH.PSTOOLS.kill_process(process_name, CONST.TEST.WS if test else workstation_name)
+            def kill_process(process_name: str, host: str) -> bool:
+                return PIH.PSTOOLS.kill_process(process_name, host)
 
-class ActionStack(List):
+            @staticmethod
+            def kill_process_via_windows(process_name: str, host: str) -> bool:
+                return PIH.PSTOOLS.kill_process_via_windows(process_name, host)
+
+class ActionStack(list):
 
     def __init__(self, caption: str = "", *argv, input: InputBase = None, output: OutputBase = None):
         self.input = input or PIH.input
         self.output = output or PIH.output
-        self.acion_value_list: List[ActionValue] = []
+        self.acion_value_list: list[ActionValue] = []
         self.caption = caption
         for arg in argv:
             self.append(arg)
         self.start()
 
     def call_actions_by_index(self, index: int = 0, change: bool = False):
         previous_change: bool = False
@@ -4149,70 +4593,87 @@
                 self.show_action_values()
 
 
 class A:
 
     root = PIH()
 
+    MH = root.MOBILE_HELPER
+
     R = root.RESULT
     D = root.DATA
     D_TN = D.TELEPHONE_NUMBER
     D_FL = D.FILTER
     D_E = D.EXTRACT
+    D_E_SPL = D_E.SERVICE_PARAMETER_LIST
     D_M = D.MARK
+    D_C = D.CHECK
     A = root.ACTION
+    A_D = A.DOCUMENTS
+    A_QR = A.QR_CODE
     A_I = A.INDICATION
     A_I_CT = A_I.CT
     ME = root.MESSAGE
+    ME_P = ME.POLIBASE
     A_WS = A.WORKSTATION
     R_ME = R.MESSAGE
-    R_RM = R.RESOURCES
+    R_R = R.RESOURCES
+    R_SSH = R.SSH
     R_I = R.INDICATIONS
+    #
     A_ME = A.MESSAGE
     A_TT = A.TIME_TRACKING
     A_MH = A.MOBILE_HELPER
     R_ME_D = R_ME.DELAYED
     A_ME_D = A_ME.DELAYED
+    
+    #
     ME_WS = ME.WORKSTATION
     ME_P = ME.POLIBASE
-    ME_P_A = ME_P.ADMIN
     ME_WH = ME.WHATSAPP
     ME_D = ME.DELAYED
     ME_WH_W = ME_WH.WAPPI
+    ME_WH_W_Q = ME_WH_W.QUEUE
+    A_ME_WH_W_Q = ME_WH_W.QUEUE
+    #
     S = root.SETTINGS
     S_U = S.USER
     S_P = S.POLIBASE
-    S_RM = S.RESOURCE_MANAGER
+    S_R = S.RESOURCE
     S_WS = S.WORKSTATION
     S_P_V = S_P.VISIT
-    S_P_R = S_P.REVIEW
+    S_P_RN = S_P.REVIEW_NOTIFICATION
+    #
     C = root.CHECK
-    C_RM = C.RESOURCE_MANAGER
+    C_R = C.RESOURCE
+    C_I = C.INDICATION
     C_M = C.MARK
     C_TT = C.TIME_TRACKING
     C_A = C.ACCESS
+    C_S = C.SETTINGS
     C_WS = C.WORKSTATION
     C_ME = C.MESSAGE
     C_ME_WH = C_ME.WHATSAPP
     C_ME_WH_W = C_ME_WH.WAPPI
+    #
     A_M = A.MARK
     R_M = R.MARK
     R_U = R.USER
     R_TT = R.TIME_TRACKING
     A_U = A.USER
     C_U = C.USER
     D_F = D.FORMAT
-    D_C = D.CHECK
+    D_CO = D.CONVERT
     A_P = A.POLIBASE
-    A_P_A = A_P.ADMIN
-    A_P_S = A_P.SETTINGS
     C_P = C.POLIBASE
+    C_P_DB = C_P.DATABASE
     D_P = D.POLIBASE
     R_P = R.POLIBASE
     R_PR = R.PRINTER
+    #
     A_P_V = A_P.VISIT
     A_P_V_DS = A_P_V.DATA_STORAGE
     R_P_V = R_P.VISIT
     R_P_V_DS = R_P_V.DATA_STORAGE
     A_P_N = A_P.NOTIFICATION
     A_P_N_C = A_P_N.CONFIRMATION
     R_P_N = R_P.NOTIFICATION
@@ -4234,10 +4695,39 @@
     A_DS = A.DATA_STORAGE
     R_DS = R.DATA_STORAGE
     V = root.VERSION
     OS = root.OS
     U = root.UPDATER
     PS = root.PSTOOLS
     E = root.ERROR
+    EV = root.EVENT
     PTH = root.PATH
+    PTH_U = PTH.USER
+    PTH_QR = PTH.QR_CODE
+    PTH_FNT = PTH.FONTS
     L = root.LOG
-    L_C = L.COMMAND
+    L_C = L.COMMAND
+
+    CT = CONST
+    CT_FNT = FONT
+    CT_SR = ServiceRoles
+    CT_SC = ServiceCommands
+    CT_F = FILE
+    CT_R = RESOURCE
+    CT_R_D = CT_R.DESCRIPTIONS
+    CT_R_IR = CT_R.INACCESSABLE_REASON
+    CT_F_E = CT_F.EXTENSION
+    CT_P = CT.POLIBASE
+    CT_P_DD = CT_P.DOCUMENT_DESCRIPTIONS
+    CT_S = SETTINGS
+    CT_ME = CT.MESSAGE
+    CT_ME_WH = CT_ME.WHATSAPP
+    CT_ME_WH_W = CT_ME_WH.WAPPI
+    CT_V = CT.VISUAL
+    CT_LC = LogCommands
+    CT_MD = MEDICAl_DOCUMENT
+    CT_MD_DT = CT_MD.DIRECTION_TYPES
+    CT_DS = CT.DATA_STORAGE
+    CT_FNC = FIELD_NAME_COLLECTION
+    CT_FCA = FIELD_COLLECTION_ALIAS
+    CT_LL = LogLevels
+    CT_AD = AD
```

### Comparing `pih-1.421/pih/rpcCommandCall_pb2.py` & `pih-1.43/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.421/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.43/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.421/pih/rpc_collection.py` & `pih-1.43/pih/rpc_collection.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 from dataclasses import dataclass
 import importlib.util
 import sys
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
-from pih.const import ServiceCommands, ServiceRoles
+from pih.const import ServiceCommands
+from pih.collection import ServiceRoleDescription
 
 
 @dataclass
 class Subscribtion:
     service_command: ServiceCommands
     type: int = None
     name: str = None
     actiated: bool = False
 
 
 @dataclass
 class Subscriber:
-    role: ServiceRoles = None
+    service_role_description: ServiceRoleDescription = None
     type: int = None
     name: str = None
     available: bool = True
     enabled: bool = True
```

### Comparing `pih-1.421/pih/tools.py` & `pih-1.43/pih/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 import re
 import string
 import random
 import json
 import os
 import subprocess
 import sys
-from typing import Any, Callable, List, Tuple
+from typing import Any, Callable, Tuple, List
 import dataclasses
+import socket
+from typing import Any
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 from pih.const import PASSWORD_GENERATION_ORDER, FIELD_COLLECTION_ALIAS
 from pih.collection import R, T, FieldItem, FieldItemList, FullName, Result, User, PolibasePerson
 
@@ -36,23 +38,23 @@
         return default_value if value not in map else map[value]
     
     @staticmethod
     def get_by_value_or_key(cls: Enum, value: Any) -> Any:
         return EnumTool.get_by_value(cls, value) or EnumTool.get(cls, value)
 
     @staticmethod
-    def get_value(value: Any, default_value: str = None) -> Any:
+    def get_value(value: Enum | Any, default_value: str = None) -> Any:
         if value is not None and isinstance(value, Enum):
             return value.value
         return value or default_value
 
 class DataTool:
 
     @staticmethod
-    def by_index(data: List, index: int, default_value: Any = None) -> Any:
+    def by_index(data: list | None, index: int, default_value: Any = None) -> Any:
         if data is None:
             return default_value
         if len(data) <= index:
             return default_value
         return data[index]
 
     @staticmethod
@@ -77,37 +79,38 @@
         def obtain_data():
             return (list(map(lambda item: DataTool.fill_data_from_source(class_type_holder(item) if callable(class_type_holder) else class_type_holder(), item), data)) if isinstance(data, list)
                     and class_type_holder is not None else DataTool.fill_data_from_source(class_type_holder(data) if callable(class_type_holder) else class_type_holder(), data) if class_type_holder is not None else data) if data is not None else None
         if "fields_alias" in result_object:
             return Result(FieldItemList(EnumTool.get(FIELD_COLLECTION_ALIAS, result_object["fields_alias"]).value), obtain_data())
         else:
             fields = None if "fields" not in result_object else result_object["fields"]
-        field_list: List[FieldItem] = None
+        field_list: list[FieldItem] = None
         if fields is not None:
             field_list = []
             for field_item in fields:
                 for field_name in field_item:
                     field_list.append(DataTool.fill_data_from_source(FieldItem(), field_item[field_name]))
         return Result(FieldItemList(field_list) if field_list else None, obtain_data())
 
     @staticmethod
-    def as_list(value: Any) -> List[Any]:
-        if isinstance(value, (List, Tuple)):
+    def as_list(value: Any) -> list[Any]:
+        if isinstance(value, (list, Tuple)):
             return value
         if DataTool.is_empty(value):
             return [] 
         return [value]
 
     @staticmethod
-    def to_list(value: Any) -> List[Any]:
-        result: List[Any] = []
+    def to_list(value: Any) -> list[Any]:
+        result: list[Any] = []
         for item in value:
             result.append(item)
         return result
 
+    @staticmethod
     def triple_bool(value: bool, false_result: Any, true_result: Any, none_reult: Any) -> Any:
         if value is None:
             return none_reult
         return true_result if value else false_result
 
     @staticmethod
     def to_result_with_fields(data: str, fields: FieldItemList, cls=None, first_data_item: bool = False) -> Result:
@@ -130,66 +133,79 @@
                 if item in source:
                     data.__setattr__(item, source[item])
         else:
             return None
         return data
 
     @staticmethod
-    def fill_data_from_list_source(class_type, source: List) -> object:
+    def fill_data_from_list_source(class_type, source: list) -> object:
         return list(map(lambda item: DataTool.fill_data_from_source(class_type(), item), source))
 
     def fill_data_from_rpc_str(data: T, source: str) -> T:
         return DataTool.fill_data_from_source(data, DataTool.rpc_unrepresent(source))
 
     @staticmethod
-    def get_first_item(value: List[T], default_value: Any = None) -> Any:
-        return DataTool.check(value is not None and len(value) > 0, lambda: value[0], default_value)
+    def get_first_item(value: list[T] | T, default_value: Any = None) -> Any:
+        return DataTool.check(value is not None and len(value) > 0, lambda: value[0], default_value) if isinstance(value, list) else value or default_value
 
     @staticmethod
     def check(check_value: bool, return_value: Callable, default_value: Any = None) -> Any:
         return return_value() if check_value else default_value
 
     @staticmethod
     def not_none_check(check_value: Any, return_value: Callable, default_value: Any = None) -> Any:
         return DataTool.check(check_value is not None, return_value, default_value() if default_value is not None and isinstance(default_value, Callable) else default_value)
 
     @staticmethod
     def if_not_none(check_value: Any, return_value: Callable[[Any], Any], default_value: Any = None) -> Any:
         return default_value if check_value is None else return_value(check_value)
 
     @staticmethod
-    def is_empty(data: Any) -> bool:
-        return data is None or (isinstance(data, (list, str, dict)) and len(data) == 0)
+    def is_empty(value: Any) -> bool:
+        return value is None or (isinstance(value, (list, str, dict)) and len(value) == 0)
+
+class ListTool:
 
+    @staticmethod
+    def not_empty_items(value: list[Any | None]) -> list[Any]:
+        return list(filter(lambda item: not DataTool.is_empty(item), value))
+    
+    @staticmethod
+    def not_less_length_items(value: list[Any | None], length: int) -> list[Any]:
+        return list(filter(lambda item: not DataTool.is_empty(item) and len(item) >= length, value))
 
 class StringTool:
 
     @staticmethod
-    def dequotes(value: str) -> Tuple[List[str], List[str]]:
-        quotes: List[str] = ["'", "\""]
-        value_list: List[str] = list(
+    def split_with_not_empty_items(value: str, symbol: str = " ") -> list[str]:
+        return ListTool.not_empty_items(value.split(symbol))
+
+    @staticmethod
+    def dequotes(value: str) -> tuple[list[str], list[str]]:
+        quotes: list[str] = ["'", "\""]
+        value_list: list[str] = list(
             filter(lambda item: not DataTool.is_empty(item), value.split(" ")))
-        result: List[str] = []
+        result: list[str] = []
         count_quote: int = value.count(quotes[0])
         count_quote2: int = value.count(quotes[1])
         if (count_quote + count_quote2) > 0:
             do_first_cut: bool = (count_quote + count_quote2) % 2 == 1
-            arg_list: List[str] = []
+            arg_list: list[str] = []
             for index, list_item in enumerate(value_list):
                 is_quoted: bool = list_item[0] in quotes
                 if is_quoted:
                     break
             arg_list = value_list[index:]
             value_list = [item for item in value_list if item not in arg_list]
             if do_first_cut:
                 for index, arg in enumerate(arg_list):
                     if arg[0] in quotes:
                         arg_list[index] = arg[1:]
                         break
-            quotes_map: List[Tuple[int, int]] = []
+            quotes_map: list[tuple[int, int]] = []
             for index, arg in enumerate(arg_list):
                 if arg[0] in quotes:
                     quotes_map.append((index, -1))
                 if arg[-1] in quotes:
                     length: int = len(quotes_map) - 1
                     quotes_map[length] = (quotes_map[length][0], index)
             for index, quote in enumerate(quotes_map):
@@ -207,25 +223,26 @@
             if len(quotes_map) > 0:
                 result += arg_list[quote[1] + 1:]
             else:
                 result += arg_list
         return value_list, result
 
     @staticmethod
-    def list_to_string(value: List, escaped_string: bool = False, separator: str = ", ", start: str = "", end: str = "", filter_empty: bool = False) -> str:
+    def list_to_string(value: list, escaped_string: bool = False, separator: str = ", ", start: str = "", end: str = "", filter_empty: bool = False) -> str:
         return start + separator.join(list(map(lambda item: f"'{item}'" if escaped_string else str(item) if item is not None else "", list(filter(lambda item: not filter_empty or not DataTool.is_empty(item), value))))) + end
 
     @staticmethod
     def capitalize(value: str) -> str:
         if DataTool.is_empty(value):
             return ""
         if len(value) == 1:
             return value[0].upper()
         return value[0].upper() + value[1:]
     
+    @staticmethod
     def decapitalize(value: str) -> str:
         if DataTool.is_empty(value):
             return ""
         return value[0].lower() + value[1:]
 
     @staticmethod
     def from_russian_keyboard_layout(value: str) -> str:
@@ -261,78 +278,91 @@
         value = self.list[self.index]
         self.index = self.index + 1
         if object is not None:
             value = DataTool.fill_data_from_source(object, value)
         return value
 
     def get(self, index: int = 0, object: Any = None, default_value: Any = None) -> Any:
-        tmp_index: int = self.index
+        temp_index: int = self.index
         self.index = index
         result: Any = self.next(object, default_value)
-        self.index = tmp_index
+        self.index = temp_index
         return result
 
     def set(self, index: int, value: Any) -> None:
         self.list[index] = value
 
 class DateTimeTool:
 
     @staticmethod
+    def yesterday() -> datetime:
+        return DateTimeTool.today(-1)
+
+    @staticmethod
+    def start_date(value: datetime | date) -> datetime | date:
+        return value.replace(hour=0, minute=0, second=0, microsecond=0) if isinstance(value, datetime) else value
+    
+    @staticmethod
+    def end_date(value: datetime | date) -> datetime | date:
+        return value.replace(hour=23, minute=59, second=59, microsecond=0) if isinstance(value, datetime) else value
+
+    @staticmethod
     def timestamp() -> int:
         return int(datetime.now().timestamp())
 
+    @staticmethod
     def date_or_today_string(date: datetime, format: str = None) -> str:
-        return DateTimeTool.to_string(date, format) if date is not None else DateTimeTool.today_string(format)
+        return DateTimeTool.datetime_to_string(date, format) if date is not None else DateTimeTool.today_string(format)
 
     @staticmethod
     def today_string(format: str = None, subtract: int = 0) -> str:
-        return DateTimeTool.to_string(DateTimeTool.today(subtract).date(), format)
+        return DateTimeTool.datetime_to_string(DateTimeTool.today(subtract).date(), format)
 
     @staticmethod
-    def to_string(date: datetime, format: str = None) -> str:
+    def datetime_to_string(date: datetime, format: str = None) -> str:
         if date is None:
             return None
         return date.isoformat() if format is None else date.strftime(format)
 
     @staticmethod
     def date_to_string(date: datetime, format: str = None) -> str:
-        return DateTimeTool.to_string(date.date(), format)
+        return DateTimeTool.datetime_to_string(date.date(), format)
 
     @staticmethod
-    def to_date_string(date: str) -> str:
-        list : List[str] = date.split("T")
+    def to_date_string(date_string: str) -> str:
+        list : list[str] = date_string.split("T")
         return list[0]
 
     @staticmethod
     def today(delta_days: int = 0) -> datetime:
         return datetime.today() + timedelta(days=delta_days)
 
     @staticmethod
     def now() -> datetime:
         return datetime.now()
 
     @staticmethod
     def now_time_string(format: str = None, delta_minutes: int = 0) -> str:
-        return DateTimeTool.to_string(DateTimeTool.now_time(delta_minutes), format)
+        return DateTimeTool.datetime_to_string(DateTimeTool.now_time(delta_minutes), format)
 
     @staticmethod
     def now_time(delta_minutes: int = 0) -> datetime:
         return datetime.combine(date.today(), datetime.now().time()) + timedelta(minutes=delta_minutes)
 
     @staticmethod
     def now_string(format: str) -> str:
-        return DateTimeTool.to_string(DateTimeTool.now(), format)
+        return DateTimeTool.datetime_to_string(DateTimeTool.now(), format)
 
     @staticmethod
     def from_string(value: str, format: str = None) -> datetime:
         return datetime.fromisoformat(value) if format is None else datetime.strptime(value, format)
 
     @staticmethod
     def is_equal_by_time(date: datetime, value: Any) -> bool:
-        if isinstance(value, tuple):
+        if isinstance(value, Tuple):
             return date.hour == value[0] and date.minute == value[1]
         if isinstance(value, datetime):
             return date.hour == value.hour and date.minute == value.minute
         return None
 
 class ResultTool:
 
@@ -342,31 +372,31 @@
         if isinstance(fields, FIELD_COLLECTION_ALIAS):
             result["fields_alias"] = fields.name
         else:
             result["fields"] = fields
         return result
 
     @staticmethod
-    def is_empty(result: Result) -> bool:
+    def is_empty(result: Result | None) -> bool:
         return result is None or DataTool.is_empty(result.data)
 
     @staticmethod
-    def get_first_element(result: Result[T], default_value: Any = None) -> T:
+    def get_first_element(result: Result[list[T] | T], default_value: Any | None = None) -> Any | T | None:
         return DataTool.get_first_item(result.data, default_value)
 
     @staticmethod
     def with_first_element(result: Result[T], default_value: Any = None) -> Result[T]:
         result.data = ResultTool.get_first_element(result, default_value)
         return result
 
     @staticmethod
     def to_string(result: Result[T], use_index: bool = True, item_separator: str = "\n", value_separator: str = None, show_caption: bool = True) -> str:
-        result_string_list: List[str] = []
-        data: List = DataTool.as_list(result.data)
-        item_result_string_list: List[str] = None
+        result_string_list: list[str] = []
+        data: list = DataTool.as_list(result.data)
+        item_result_string_list: list[str] = None
         for index, data_item in enumerate(data):
             if use_index and len(data) > 1:
                 result_string_list.append(f"*{str(index + 1)}*:")
             if value_separator is not None:
                 item_result_string_list = []
             for field_item in result.fields.list:
                 field: FieldItem = field_item
@@ -389,66 +419,78 @@
                     else:
                         item_result_string_list.append(data_value)
             if value_separator is not None:
                 result_string_list.append(value_separator.join(item_result_string_list))
         return item_separator.join(result_string_list)
 
     @staticmethod 
-    def as_list(result: Result[T]) -> Result[List[T]]:
-        return Result(result.fields, [] if result.data is None else [result.data] if not isinstance(result.data, List) else result.data)
+    def as_list(result: Result[T]) -> Result[list[T]]:
+        return Result(result.fields, [] if result.data is None else [result.data] if not isinstance(result.data, list) else result.data)
 
     @staticmethod
-    def filter(result: Result[List[T]], filter_function: Callable) -> Result[List[T]]:
+    def filter(result: Result[list[T]], filter_function: Callable) -> Result[list[T]]:
         if filter_function is not None:
             try:
                 result.data = list(filter(filter_function, result.data))
             except StopIteration:
                pass 
         return result
 
     @staticmethod
-    def sort(result: Result[List[T]], sort_function: Callable) -> Result[List[T]]:
+    def sort(result: Result[list[T]], sort_function: Callable) -> Result[list[T]]:
         if sort_function is not None:
             result.data.sort(key=sort_function)
         return result
 
 
     @staticmethod
-    def every(result: Result[List[T]], action_function: Callable[[T], None]) -> Result[List[T]]:
+    def every(result: Result[list[T]], action_function: Callable[[T], None]) -> Result[list[T]]:
         for item in result.data:
             action_function(item)
         return result
+    
+    @staticmethod
+    def do_while(result: Result[list[T]], check_function: Callable[[T], bool]) -> Any | None:
+        result_data: Any | None = None
+        for item in result.data:
+            if check_function(item):
+                result_data = item
+                break
+        return result_data
 
     @staticmethod
-    def map(result: Result[List[T]], map_function: Callable[[T], R], map_on_each_data_item: bool = True) -> Result[List[R]]:
+    def map(result: Result[list[T]], map_function: Callable[[T], R], map_on_each_data_item: bool = True) -> Result[list[R]]:
         result.data = list(map(map_function, result.data)
                            ) if map_on_each_data_item else map_function(result.data)
         return result
 
 class TranslateTool:
 
+    @staticmethod
     def ru_to_en(value: str) -> str:
         return value.translate(dict(zip(map(ord,  
         "йцукенгшщзхъфывапролджэячсмитьбю.ё"
         'ЙЦУКЕНГШЩЗХЪФЫВАПРОЛДЖЭЯЧСМИТЬБЮ,Ё'),
         "qwertyuiop[]asdfghjkl;'zxcvbnm,./`"
         'QWERTYUIOP{}ASDFGHJKL:"ZXCVBNM<>?~')))
 
 class BitMask:
 
     @staticmethod
     def set(value: int, bit: Any) -> int:
-        bits: List[int] = bit if isinstance(bit, list) else [bit]
+        bits: list[int] = bit if isinstance(bit, list) else [bit]
         for bit in bits:
             value |= bit
         return value
 
     @staticmethod
     def has(value: int, bit: Any) -> bool:
-        bits: List[int] = bit if isinstance(bit, list) else [bit]
+        if value is None:
+            return False
+        bits: list[int] = bit if isinstance(bit, list) else [bit]
         result: bool = False
         if len(bits) > 1:
             for bit in bits:
                 result = BitMask.has(value, bit)
                 if result:
                     break
         else:
@@ -463,15 +505,15 @@
         if BitMask.has(value, bit):
             value ^= bit
         return value
 
 class ResultUnpack:
 
     @staticmethod
-    def unpack(result: dict) -> Tuple[FieldItemList, Any]:
+    def unpack(result: dict) -> tuple[FieldItemList, Any]:
         return ResultUnpack.unpack_fields(result), ResultUnpack.unpack_data(result)
 
     @staticmethod
     def unpack_fields(data: dict) -> Any:
         if "fields_alias" in data:
             return FIELD_COLLECTION_ALIAS._member_map_[data["fields_alias"]].value,
         return data["fields"]
@@ -512,18 +554,25 @@
         head, tail = ntpath.split(path)
         value = tail or ntpath.basename(head)
         if not with_extension:
             value = value[0: value.rfind(".")]
         return value
 
     @staticmethod
+    def get_file_directory(path: str):
+        head, tail = ntpath.split(path)
+        if head[-1] in ["\\", "/"]:
+            head = head[:-1]
+        return head
+
+    @staticmethod
     def get_extension(file_path: str, ) -> str:
-        dot_index: int = file_path.find(".")
+        dot_index: int = file_path.rfind(".")
         if dot_index != -1:
-            return file_path[dot_index + 1:]
+            return file_path[dot_index + 1:].lower()
         return ""
 
     @staticmethod
     def replace_prohibited_symbols_from_path_with_symbol(path: str, replaced_symbol: str = "_") -> str:
         return path.replace("\\", replaced_symbol).replace("/", replaced_symbol).replace("?", replaced_symbol).replace("<", replaced_symbol).replace(">", replaced_symbol).replace("*", replaced_symbol).replace(":", replaced_symbol).replace("\"", replaced_symbol)
 
     @staticmethod
@@ -556,19 +605,27 @@
 
     @staticmethod
     def is_accessable(host_or_ip: str, packets: int = 1, timeout: int = 100):
         if platform.system().lower() == "windows":
             command = ["ping", "-4", "-n", str(packets), "-w", str(timeout), host_or_ip]
             result = subprocess.run(command, stdin=subprocess.DEVNULL, stdout=subprocess.PIPE,
                                     stderr=subprocess.DEVNULL, creationflags=0x08000000)
-            return result.returncode == 0 and b"TTL=" in result.stdout
+            out: str = str(result.stdout, "unicode_escape")
+            return result.returncode == 0 and (int(str(out.split(" = ")[-3:][2]).splitlines()[0]) < packets and out.count("(TTL)") < packets)
         else:
             command = ["ping", "-c", str(packets), "-w", str(timeout), host_or_ip]
             result = subprocess.run(command, stdin=subprocess.DEVNULL, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
             return result.returncode == 0
+
+    @staticmethod
+    def next_free_port() -> int:
+        with socket.socket() as soc:
+            soc.bind(('', 0))
+            return soc.getsockname()[1]
+        
         
 class FullNameTool:
 
     SPLIT_SYMBOL: str = " "
     FULL_NAME_LENGTH: int = 3
 
     @staticmethod
@@ -578,55 +635,48 @@
     @staticmethod
     def to_given_name(full_name_holder: Any, join_symbol: str = SPLIT_SYMBOL) -> str:
         if isinstance(full_name_holder, PolibasePerson):
             return FullNameTool.to_given_name(full_name_holder.FullName)
         if isinstance(full_name_holder, User):
             return FullNameTool.to_given_name(full_name_holder.name)
         if isinstance(full_name_holder, FullName):
-            return join_symbol.join(list(filter(lambda item: len(item) > 0, [full_name_holder.first_name, full_name_holder.middle_name])))
+            return join_symbol.join(ListTool.not_empty_items([full_name_holder.first_name, full_name_holder.middle_name]))
         elif isinstance(full_name_holder, str):
             full_name_holder = full_name_holder.strip()
             if FullNameTool.is_full_name(full_name_holder):
                 return FullNameTool.to_given_name(FullNameTool.from_string(full_name_holder, join_symbol))
             else:
                 return full_name_holder
 
     @staticmethod
     def from_string(value: str, split_symbol: str = SPLIT_SYMBOL) -> FullName:
-        full_name_string_list: List[str] = list(filter(lambda item: len(item) > 0, value.split(split_symbol)))
+        full_name_string_list: list[str] = ListTool.not_empty_items(value.split(split_symbol))
         return FullName(full_name_string_list[0], full_name_string_list[1], full_name_string_list[2])
 
     @staticmethod
     def is_full_name(value: str, split_symbol: str = SPLIT_SYMBOL) -> bool:
-        return len(list(filter(lambda item: len(item) > 0, value.split(split_symbol)))) >= FullNameTool.FULL_NAME_LENGTH
+        return len(ListTool.not_empty_items(value.split(split_symbol))) >= FullNameTool.FULL_NAME_LENGTH
 
     @staticmethod
     def is_equal(fn_a: FullName, fn_b: FullName) -> bool:
         return fn_a.first_name == fn_b.first_name and fn_a.middle_name == fn_b.middle_name and fn_a.last_name == fn_b.last_name
 
     @staticmethod
     def is_intersect(fn_a: FullName, fn_b: FullName) -> bool:
-        al: List[str] = [fn_a.last_name, fn_a.first_name, fn_a.middle_name]
-        bl: List[str] = [fn_b.last_name, fn_b.first_name, fn_b.middle_name]
+        al: list[str] = [fn_a.last_name, fn_a.first_name, fn_a.middle_name]
+        bl: list[str] = [fn_b.last_name, fn_b.first_name, fn_b.middle_name]
         return len([value for value in al if value in bl]) == FullNameTool.FULL_NAME_LENGTH
 
 class Clipboard:
 
     @staticmethod
     def copy(value: str):
         import pyperclip as pc
         pc.copy(value)
 
-    '''
-    @staticmethod
-    def copy(value: str):
-        cmd = 'echo '+value.strip()+'|clip'
-        return subprocess.check_call(cmd, shell=True)
-    '''
-
 class UserTools:
 
     @staticmethod
     def get_given_name(user: User) -> str:
         return FullNameTool.to_given_name(user.name)
 
 class PasswordTools:
@@ -635,51 +685,38 @@
     def check_password(value: str, length: int, special_characters: str) -> bool:
         regexp_string = "^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[" + special_characters + \
             "])[A-Za-z\d" + special_characters + "]{" + str(length) + ",}$"
         password_checker = re.compile(regexp_string)
         return re.fullmatch(password_checker, value) is not None
 
     @staticmethod
-    def generate_random_password(length: int, special_characters: str, order_list: List[str], special_characters_count: int, alphabets_lowercase_count: int, alphabets_uppercase_count: int, digits_count: int, shuffled: bool):
-        # characters to generate password from
+    def generate_random_password(length: int, special_characters: str, order_list: list[str], special_characters_count: int, alphabets_lowercase_count: int, alphabets_uppercase_count: int, digits_count: int, shuffled: bool):
         alphabets_lowercase = list(string.ascii_lowercase)
         alphabets_uppercase = list(string.ascii_uppercase)
         digits = list(string.digits)
         characters = list(string.ascii_letters +
                           string.digits + special_characters)
         characters_count = alphabets_lowercase_count + \
             alphabets_uppercase_count + digits_count + special_characters_count
-        # check the total length with characters sum count
-        # print not valid if the sum is greater than length
         if characters_count > length:
             return
-        # initializing the password
-        password: List[str] = []
+        password: list[str] = []
         for order_item in order_list:
             if order_item == PASSWORD_GENERATION_ORDER.SPECIAL_CHARACTER:
-             # picking random alphabets
                 for i in range(special_characters_count):
                     password.append(random.choice(special_characters))
             elif order_item == PASSWORD_GENERATION_ORDER.LOWERCASE_ALPHABET:
-                # picking random lowercase alphabets
                 for i in range(alphabets_lowercase_count):
                     password.append(random.choice(alphabets_lowercase))
             elif order_item == PASSWORD_GENERATION_ORDER.UPPERCASE_ALPHABET:
-                # picking random lowercase alphabets
                 for i in range(alphabets_uppercase_count):
                     password.append(random.choice(alphabets_uppercase))
             elif order_item == PASSWORD_GENERATION_ORDER.DIGIT:
-                # picking random digits
                 for i in range(digits_count):
                     password.append(random.choice(digits))
-        # if the total characters count is less than the password length
-        # add random characters to make it equal to the length
         if characters_count < length:
             random.shuffle(characters)
             for i in range(length - characters_count):
                 password.append(random.choice(characters))
-        # shuffling the resultant password
         if shuffled:
             random.shuffle(password)
-        # converting the list to string
-        # printing the list
-        return "".join(password)
+        return "".join(password)
```

### Comparing `pih-1.421/pih/widgets.py` & `pih-1.43/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.421/pih_setup.py` & `pih-1.43/pih_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,25 +65,26 @@
 for filename in os.listdir(folder):
     file_path = os.path.join(folder, filename)
     try:
         if os.path.isfile(file_path) or os.path.islink(file_path):
             os.unlink(file_path)
         elif os.path.isdir(file_path):
             shutil.rmtree(file_path)
-    except Exception as e:
-        print('Failed to delete %s. Reason: %s' % (file_path, e))
+    except Exception as error:
+        print("Failed to delete %s. Reason: %s" % (file_path, error))
 
-# This call to setup() does all the work
+#This call to setup() does all the work
 setup(
     name=PIH.NAME,
     version=f"{PIH.VERSION.local()}",
     description="PIH library",
     long_description_content_type="text/markdown",
     url="https://pacifichosp.com/",
     author="Nikita Karachentsev",
     author_email="it@pacifichosp.com",
     license="MIT",
     classifiers=[],
     packages=[PIH.NAME],
     include_package_data=True,
-    install_requires=["prettytable", "colorama", "grpcio", "protobuf", "requests", "transliterate"]
+    install_requires=["prettytable", "colorama", "grpcio",
+                      "protobuf", "requests", "transliterate", "psutil"]
 )
```

