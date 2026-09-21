# PyTorch Learning

Ноутбуки по изучению PyTorch. Каждый файл — отдельная тема: краткая теория и рабочий код с проверками shape/dtype на каждом шаге.

## Содержание

| # | Ноутбук | Тема |
|---|---------|------|
| 1 | [`PyTorch1.ipynb`](PyTorch1.ipynb) | Подготовка данных: `Dataset`, `DataLoader`, трансформации |
| 2 | [`PyTorch2.ipynb`](PyTorch2.ipynb) | Первые нейросети: `nn.Module` и цикл обучения |

## Описание ноутбуков

### 1. PyTorch1 — подготовка данных
Как превратить файлы с диска в батчи тензоров. Задачи: классификация (MNIST по папкам) и регрессия (синтетические картинки с квадратом, предсказание координат центра). Разбираются собственные `Dataset` и `ImageFolder`, `random_split`, `DataLoader`, трансформации `transforms` / `transforms.v2` и собственная трансформация через `torch.nn.Module`.

### 2. PyTorch2 — первые нейросети и цикл обучения
Построение моделей и их обучение на данных из первого ноутбука. Способы задать модель: `nn.Sequential`, собственный класс `nn.Module`, `ModuleList` / `ModuleDict`, модели с несколькими входами и выходами. Далее полный цикл обучения (прямой проход, ошибка, `backward`, шаг оптимизатора, валидация, метрики, графики loss/accuracy) на двух задачах: классификация MNIST (`CrossEntropyLoss`, Adam) и регрессия координат (`MSELoss`). Перенос модели и данных на GPU.

## Установка

```bash
git clone https://github.com/Aleks-Kuzo/<repo-name>.git
cd <repo-name>
pip install torch torchvision numpy matplotlib pillow jupyter
```

Python 3.9+, `torchvision` ≥ 0.16. В ноутбуках используются локальные пути к данным — замените их на свои.
