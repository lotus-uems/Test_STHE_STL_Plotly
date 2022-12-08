# Test_STHE_STL_Plotly
Задача:
-------

![alt text](https://github.com/lotus-uems/Test_STHE_STL_Plotly/blob/main/sthe_stl_model_22606154.png)

На входе у вас есть следующие данные:
1. 3Д-модель кожухотрубного теплообменника в формате .STL
2. Массив данных по температурам внутри данного теплообменника (возьмите просто случайные данные)
3. Функция на Python, которая по координатам (x, y ,z) выдает температуру (функцию напишите сами, пусть выдает пока просто случайные данные)

Необходимо:
1. Перевести модель .STL в формат plotly.Mesh (это уже реализовано в прилагаемом ноутбуке)
Для исправления эффекта сплющивания используйте код:
```
layout = go.Layout(
    paper_bgcolor='rgb(1,1,1)',
    title_text=title,
    title_x=0.5,
    font_color='white',
    width=1600,
    height=800,
    scene_camera=dict(
        eye=dict(x=1.25, y=1.25, z=1)),
    scene_xaxis_visible=True,
    scene_yaxis_visible=True,
    scene_zaxis_visible=True,
    scene = dict(aspectratio = dict(
        x = 4,
        y = 1,
        z = 1
    )),
)
```
2. Наложить на полученную визуализацию в plotly данные по температурам

Ноутбук для выполнения задания: https://colab.research.google.com/drive/1gHpfqoH9zBo_HrIOLLe_oIYEe0xNJ-En?usp=sharing

Пример визуализация данных по температурам:

![alt text](https://github.com/lotus-uems/Test_STHE_STL_Plotly/blob/main/22606154_ShellTemps.png) 

Пример уже совмещенной визуализации данных в 3Д модели:

![alt text](https://github.com/lotus-uems/Test_STHE_STL_Plotly/blob/main/22606154_ShellTemps_in_STL.png) 

Для связи по всем вопросам, пишите в телеграм: @TAU15

Выполненное задание отправьте, пожалуйста, через эту форму: https://airtable.com/shrkZvrZGEVlzle5m
