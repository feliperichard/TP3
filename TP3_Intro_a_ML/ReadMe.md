Como disponibilizar el entorno para el trabajo práctico.

1. Recomendamos se installe una distribución de conda ( en esta etapa con miniconda debería bastar ) puede consultar la instalación [la página del proyecto](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)

2. Instale el entorno con dependencias básicas para ejecutar el proyecto

Vaya a la carpeta del trabajo prácticp
```sh
cd TP3_Intro_a_ML
```

e instale el entorno y sus dependencias
```sh
conda env create -f environment.yml
```

3. active el entorno de desarrollo para este trabajo práctico `ddatos21_ment_tp3` ( en lo sucesivo será ddatos21_ment_tp2, ddatos21_ment_tp3, etc )

```sh
conda activate ddatos21_ment_tp3
```
4. Ejecute jupyter a fin de poder ejecutar las notebooks

```sh
jupyter notebook --ip='*' --NotebookApp.token='' --NotebookApp.password=''
```

5. El enunciado del proyecto debería estar en [EnunciadoTP3IntroML.ipynb](http://localhost:8888/notebooks/EnunciadoTP3IntroML.ipynb)

6. En caso de actualizar dependencias puede cambiar el archivo  environment.yml
```sh
conda env update --file environment.yml --prune
```