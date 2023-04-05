# hse_hw3_chromhmm

## Ссылка на колаб

https://colab.research.google.com/drive/1Yb6NJBZ3dExwsr5jfzeUXepEV0Aa582W?usp=sharing

## Клеточная линия и гистоновые метки

Как и в прошлом ДЗ я выбрал клеточную линию HeLa-S3. Для нее я буду анализировать следующие гистоновые метки:
- H2az (wgEncodeBroadHistoneHelas3H2azAlnRep1.bam)
- H3k27ac (wgEncodeBroadHistoneHelas3H3k27acStdAlnRep1.bam)
- H3k27me3 (wgEncodeBroadHistoneHelas3H3k27me3StdAlnRep1.bam)
- H3k36me3 (wgEncodeBroadHistoneHelas3H3k36me3StdAlnRep1.bam)
- H3k04me1 (wgEncodeBroadHistoneHelas3H3k04me1StdAlnRep1.bam)
- H3k4me2 (wgEncodeBroadHistoneHelas3H3k4me2StdAlnRep1.bam)
- H3k4me3 (wgEncodeBroadHistoneHelas3H3k4me3StdAlnRep1.bam)
- H3k79me2 (wgEncodeBroadHistoneHelas3H3k79me2StdAlnRep1.bam)
- H3k9ac (wgEncodeBroadHistoneHelas3H3k9acStdAlnRep1.bam)
- H3k09me3 (wgEncodeBroadHistoneHelas3H3k09me3AlnRep1.bam)

А также был использован контрольный файл wgEncodeBroadHistoneHelas3ControlStdAlnRep1.bam

## Содержание cellmarkfiletable.txt

```
Helas3	H2az	H2az.bam	сontrol.bam
Helas3	H3k27ac	H3k27ac.bam	сontrol.bam
Helas3	H3k27me3	H3k27me3.bam	сontrol.bam
Helas3	H3k36me3	H3k36me3.bam	сontrol.bam
Helas3	H3k04me1	H3k04me1.bam	сontrol.bam
Helas3	H3k4me2	H3k4me2.bam	сontrol.bam
Helas3	H3k4me3	H3k4me3.bam	сontrol.bam
Helas3	H3k79me2	H3k79me2.bam	сontrol.bam
Helas3	H3k9ac	H3k9ac.bam	сontrol.bam
Helas3	H3k09me3	H3k09me3.bam	сontrol.bam
```

## Результаты работы ChromHMM

![image](https://user-images.githubusercontent.com/87883391/230109719-0d346c4e-9523-4f44-8629-2c5546d12158.png)
![image](https://user-images.githubusercontent.com/87883391/230109845-76e819b7-1915-4e5d-b94d-18036e6b7c26.png)
![image](https://user-images.githubusercontent.com/87883391/230109925-4047b3ac-ec38-45a0-b521-321af96a334f.png)
![image](https://user-images.githubusercontent.com/87883391/230109974-2a4e9eb2-b98c-4098-8ee3-805308861fb2.png)
![image](https://user-images.githubusercontent.com/87883391/230110050-608799ff-13df-4937-ad34-8571cab9622c.png)

## Таблица

| Номер типа | Название | Обоснование |
|----------|----------|----------|
| 1    | Weak enhancer   | Попадает на ген, на интроны. Выражен в основном в H3K4me1   |
| 2    | Weak enhancer   | Попадает на ген, на интроны. В основном выражен в H3K4me1, H3K4me2, H3K27ac   |
| 3    | Active promoter   | Часто попадает на CpG островки   |
| 4    | Active promoter   | Часто попадает на CpG островки   |
| 5    | Weak transcribed   | Попадает на гены, их интроны и экзоны. В основном выражен в H3K79me2 и H3K4me2   |
| 6    | Weak enhancer   | Попадает на ген, на интроны. Выражен в H3K79me2   |
| 7    | Repressed   | Не попадает на ген, никакие гистоновые метки не выражены    |
| 8    | Weak transcribed   | Попадает на гены, их интроны и экзоны. Выражен только в H3K36me3   |
| 9    | Heterochromatin   | Чаще всего находится на ядерной ламине   |
| 10    | Heterochromatin   | Чаще всего находится на ядерной ламине   |

## Скриншоты из Genome Browser

![image](https://user-images.githubusercontent.com/87883391/230199636-44f47350-35f1-499e-8dc4-3b6428f0ff1b.png)
![image](https://user-images.githubusercontent.com/87883391/230200652-0b8da3b5-c80b-4401-a636-904e24d85391.png)
![image](https://user-images.githubusercontent.com/87883391/230204937-c529ee1e-649e-4799-a083-7421be8fbd2d.png)

## Бонус

Код для решения бонуса приведен в колаб ноутбуке
