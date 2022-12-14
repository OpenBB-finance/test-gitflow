---
title: type
description: OpenBB Terminal Function
---

# type

Show the type of the columns of the dataset and/or change the type of the column

### Usage

```python
type [-n {}] [--format {int,float,str,bool,category,date}]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| name | Provide dataset.column series to change type or dataset to see types. | None | True | None |
| format | Set the format for the dataset.column defined. This can be: date, int, float, str, bool or category | None | True | int, float, str, bool, category, date |


---

## Examples

```python
txt
2022 Feb 28, 15:53 (๐ฆ) /econometrics/ $ load wage_panel -a wp

2022 Feb 28, 15:53 (๐ฆ) /econometrics/ $ type
           wp
โโโโโโโโโโโโโโณโโโโโโโโโโ
โ column     โ dtype   โ
โกโโโโโโโโโโโโโโโโโโโโโโโฉ
โ nr         โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ year       โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ black      โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ exper      โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ hisp       โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ hours      โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ married    โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ educ       โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ union      โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ lwage      โ float64 โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ expersq    โ int64   โ
โโโโโโโโโโโโโโผโโโโโโโโโโค
โ occupation โ int64   โ
โโโโโโโโโโโโโโดโโโโโโโโโโ
```
---
