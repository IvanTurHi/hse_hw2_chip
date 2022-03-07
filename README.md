# hse_hw2_chip

# рассмотрим отчеты FastQC по файлам

|  | Реплика 1| Реплика 2 | Контроль |
| :---: | :---: | :---: | :---: |
| Basic Statistics | ![image](https://user-images.githubusercontent.com/65420132/157093733-8e774679-797c-4a0a-9490-dbccb77bd5ad.png)|![image](https://user-images.githubusercontent.com/65420132/157093759-d17d7b37-0ee6-49bf-b0de-a3436579062b.png) | ![image](https://user-images.githubusercontent.com/65420132/157093785-b266c520-b082-4f2e-b70c-a8307a1a7deb.png) |
| Basic Statistics | ![image](https://user-images.githubusercontent.com/65420132/157091498-f45f826a-a4ab-4e4d-bd16-c423776803a5.png) |![image](https://user-images.githubusercontent.com/65420132/157091640-2a718c46-8320-47f5-914b-07c322b49c2c.png) | ![image](https://user-images.githubusercontent.com/65420132/157091691-2cf9ddbe-c613-401d-b04a-1aeb87dd5b47.png) |
| Per base sequence quality | ![image](https://user-images.githubusercontent.com/65420132/157092272-e1027ccb-1177-4d2e-afc4-e0f25bf9209c.png) | ![image](https://user-images.githubusercontent.com/65420132/157092304-d03dba51-a713-48d9-ae9e-8628c39c7919.png) | ![image](https://user-images.githubusercontent.com/65420132/157092346-f07070c4-89aa-42c4-aa16-fcd8b5433149.png) |
| Per tile sequence quality | ![image](https://user-images.githubusercontent.com/65420132/157092163-5589965a-699d-46ab-8b38-86fddc62d6e1.png) | ![image](https://user-images.githubusercontent.com/65420132/157092204-c9cee649-be75-4e34-8493-64956073d2ce.png) | ![image](https://user-images.githubusercontent.com/65420132/157092236-e28c0fc7-bfcf-4b3c-969d-88e33b66de3d.png) |
| Per sequence quality scores |![image](https://user-images.githubusercontent.com/65420132/157092385-c02e37b0-4f17-405a-bcee-8a931493f530.png)| ![image](https://user-images.githubusercontent.com/65420132/157092431-b8aac36c-1242-414a-874d-c2b34324360e.png) | ![image](https://user-images.githubusercontent.com/65420132/157092472-a59aa741-99ad-4c76-96c2-773667ef464b.png) |
| Per sequence GC content | ![image](https://user-images.githubusercontent.com/65420132/157093086-bf0d9f69-fd5f-4d02-b78f-be5d5590021c.png)| ![image](https://user-images.githubusercontent.com/65420132/157093117-dd8ea578-0efd-4f83-91d0-ba8cc3adbff2.png) | ![image](https://user-images.githubusercontent.com/65420132/157093145-3b5f661f-8e38-4af3-a476-db4bd600b300.png) |
| Overrepresented sequences | ![image](https://user-images.githubusercontent.com/65420132/157093177-07a898af-dfdb-4d0a-bbfa-0814f0ddbe6d.png) | ![image](https://user-images.githubusercontent.com/65420132/157093194-f5bda840-fa10-4855-91b0-b9b8f1669a91.png) | ![image](https://user-images.githubusercontent.com/65420132/157093219-8e79ceee-616c-4e2a-ab95-f1a909bae5ea.png) |
| Adapter Content | ![image](https://user-images.githubusercontent.com/65420132/157093251-5f24653b-64c9-4465-b733-8d4495ae4694.png) | ![image](https://user-images.githubusercontent.com/65420132/157093278-20d91b53-9e00-4f79-bc37-da9e7db9ed8c.png) | ![image](https://user-images.githubusercontent.com/65420132/157093307-9f467f4b-678b-4f72-b8c4-f3cc9581793a.png) |

По отчетам видно, что качество чтений Реплики 2 и контроля высокое и никакая дальнейшая обработка файлов не требуется. Качество реплики 1 не настолько хорошее, однако все равно достаточно высокое и находится в нужных значениях. Из этого можно сделать вывод, что дальнейшая фильтрация не требуется.

# Анализ выравнивания

|  | Реплика 1 | Реплика 2 | Контроль |
| :---: | :---: | :---: | :---: |
| Общее количество ридов | 33658684 | 68989250 | 10508255 |
| Вырвнялись уникально | 1685030 / 5.01% | 3658433 / 5.30% | 617520 / 5.88% |
| Выровнялись не уникально | 3088416 / 9.18% | 7011222 / 10.16% | 1079187 / 10.27% |
| Не выровнялись |28885238 / 85.82% | 58319595 / 84.53% | 8811548 / 83.85% |
