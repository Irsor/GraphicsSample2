# Шаблон проекта по компьютерной графике. Версия № 2

Этот проект позволяет собрать приложения с использованием библиотек ```GLFW```, ```GLAD```, ```stb_image```, ```Dear ImGui``` и ```GLM``` средствами ```CMake```.

## Установка

```bash
git clone --recursive https://github.com/Irsor/Graphics-Template.git
```

## Запуск

Изменить занчения поля ```configurations/program``` на название программы в файле ```launch.json```.
Изменить значение переменной ```PROJECT_NAME``` в файле ```CMakeLists.txt ``` на название программы.

## Обновление бибилотек кроме ```GLAD```

```bash
git pull
git submodule update --recursive
```
