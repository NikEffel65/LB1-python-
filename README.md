# LB1-python-

# Архиватор/Распаковщик (bz2 и zstd)

Консольная утилита для сжатия и распаковки файлов с поддержкой алгоритмов bz2 и zstd.

## Требования
- Python 3.11+ (для встроенного zstd) или Python 3.6+ с установленным zstandard
- Для zstd в Python < 3.11: `pip install zstandard`

# Сжатие одиночного файла в bz2
python lb1.py compress file.txt archive.bz2

# Сжатие одиночного файла в zst (если доступно)
python lb1.py compress file.txt archive.zst

# Сжатие папки в tar.bz2
python lb1.py compress folder/ archive.tar.bz2

# Сжатие папки в tar.zst
python lb1.py compress folder/ archive.tar.zst

# С прогресс-баром
python lb1.py compress file.txt archive.bz2 --progress

# С замером времени
python lb1.py compress file.txt archive.bz2 --benchmark

# С прогресс-баром и замером времени
python lb1.py compress file.txt archive.bz2 --progress --benchmark

### **Скриншот 1: Архивация файла(bz2)**
<img width="1288" height="436" alt="2025-12-16_21-12-15" src="https://github.com/user-attachments/assets/7bdd5280-fc42-4217-9fe3-81ce35884cfa" />

### **Скриншот 2: Распаковка файла(bz2)**
<img width="654" height="52" alt="2025-12-16_21-15-56" src="https://github.com/user-attachments/assets/905fcc9a-63b1-41a9-bb6d-4b32401032cd" />

### **Скриншот 3: Архивация файла(zst)**
<img width="1631" height="458" alt="2025-12-16_21-50-19" src="https://github.com/user-attachments/assets/b0190809-1abe-4330-b757-18caf682050c" />

### **Скриншот 4: Распаковка директории(zst)**
<img width="1920" height="422" alt="2025-12-16_21-52-31" src="https://github.com/user-attachments/assets/50711ce9-f523-4614-bd0a-456ae773f421" />




