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

### **Скриншот 1: Архивация файла**
<img width="1288" height="436" alt="2025-12-16_21-12-15" src="https://github.com/user-attachments/assets/7bdd5280-fc42-4217-9fe3-81ce35884cfa" />

### **Скриншот 2: Распаковка файла**
<img width="654" height="52" alt="2025-12-16_21-15-56" src="https://github.com/user-attachments/assets/905fcc9a-63b1-41a9-bb6d-4b32401032cd" />

### **Скриншот 3: Архивация директории**
<img width="1815" height="848" alt="2025-12-16_21-18-57" src="https://github.com/user-attachments/assets/d2965e2d-b8ae-4890-b455-275d6275d467" />

### **Скриншот 4: Распаковка директории**
<img width="1920" height="448" alt="2025-12-16_21-20-35" src="https://github.com/user-attachments/assets/27a9c165-d4e8-481a-b3a1-897183d4094d" />



