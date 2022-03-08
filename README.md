# hse_hw2_chip

# Ссылка на колаб  
https://colab.research.google.com/drive/1bbKq4nKB0Wf3mq06VFC1D0aS7xgV70yq?usp=sharing

# Рассмотрим отчеты FastQC по файлам

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

Вопрос: Проанализируйте выдачу bowtie. Почему процент выравниваний получился именно таким?  
Ответ: Выравнивание производилось только на одну хромосому, поэтому общий процент выровненных ридов достаточно низкий. В то же время 

# Анализ диаграмм

|  | Сравнение реплики с образцом| Сравнение образца с репликой |
| :---: | :---: | :---: |
| Реплика 1 | ![image](https://user-images.githubusercontent.com/65420132/157119228-9a31196a-3bec-4f79-95e7-b8246f1fbb2e.png) | ![image](https://user-images.githubusercontent.com/65420132/157119276-0cf88115-b0c3-4518-8040-c0e6cd5685f5.png) |
| Реплика 2 | ![image](https://user-images.githubusercontent.com/65420132/157119030-cb0e10d1-81ad-4b16-b215-bf429eaabf8d.png)  | ![image](https://user-images.githubusercontent.com/65420132/157119090-7bb5fae1-fc8f-48df-94a7-69cf6d5ad2e6.png) |

У нас достаточно мало пиков из-за выравнивания всего на одну хромосому, поэтому количество пересечений и вовсе маленькое. Наблюдаемая разница в количестве пересечений при замене порядка подаваемых множеств происходит из-за того, что считается количество компонентов первого множества, которые есть во втором. При этом можно видеть, что при поиске пересечений для файлов с пиками значения получаются больше. Возможно это связано с тем, что эти пики мы и искали, поэтому их наличие в файле образца относительно ожидаемо. При обратной же ситуации мы смотрим на все фрагменты образца и не удивительно, что в файле с пиками их меньше.

# Бонусное задание

Рассмотрим нашу гистоновую метку H3K4me2
![image](https://user-images.githubusercontent.com/65420132/157246402-d28a0879-bb2b-478d-8769-e2fded65b722.png)

Посмотрим на графики, которые у нас получились:

|  | ngs | Heatmap |
| :---: | :---: | :---: |
| ENCFF076UJA| ![image](https://user-images.githubusercontent.com/65420132/157247365-969f9805-850d-43ae-b44e-a1002a8d13dc.png) | ![image](https://user-images.githubusercontent.com/65420132/157247407-d5086e4a-7be2-4958-962a-07f5e7546cce.png) |
| ENCFF346CYG| ![image](https://user-images.githubusercontent.com/65420132/157247288-96b3442a-def1-4c82-bd81-a5475e13e974.png) | ![image](https://user-images.githubusercontent.com/65420132/157247333-c112f26d-9383-4b3f-a8e8-1c999cc0c5ad.png) |

В нашем случае, активность смещена в левый край, что видно по графикам и heatmap, в то время как на картинке пики приходится на центр.
