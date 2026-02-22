## 学習項目

- DS pandas, numpy, Seabornを活用できる力を養う

## 初めのコンテナ動かす方法

```
docker run -it \
  -p 8889:8889 \
  --platform linux/amd64 \
  --name python_data_analysis \
  -v "$(pwd):/work" \
  datascientistus/ds-python-env \
  jupyter lab --ip=0.0.0.0 --allow-root --port=8889 \
  --NotebookApp.token='' \
  --notebook-dir=/work
```

2回目以降

```
docker start -i python_data_analysis
```
# python-data-analysis
