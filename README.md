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

