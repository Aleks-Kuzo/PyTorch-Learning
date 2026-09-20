# PyTorch Learning 

Ноутбуки по изучению PyTorch. Каждый файл — отдельная тема: краткая теория и рабочий код с проверками shape/dtype на каждом шаге.

## Содержание

| # | Ноутбук | Тема |
|---|---------|------|
| 1 | [`PyTorch1.ipynb`](PyTorch1.ipynb) | Подготовка данных: `Dataset`, `DataLoader`, трансформации |

## Описание ноутбуков

### 1. PyTorch1 — подготовка данных
Как превратить файлы с диска в батчи тензоров. Задачи: классификация (MNIST по папкам) и регрессия (синтетические картинки с квадратом, предсказание координат центра). Разбираются собственные `Dataset` и `ImageFolder`, `random_split`, `DataLoader`, трансформации `transforms` / `transforms.v2` и собственная трансформация через `torch.nn.Module`.

## Установка

```bash
git clone https://github.com/Aleks-Kuzo/<repo-name>.git
cd <repo-name>
pip install torch torchvision numpy matplotlib pillow jupyter
```

Python 3.9+, `torchvision` ≥ 0.16. В ноутбуках используются локальные пути к данным — замените их на свои.
