#### Requirements
Install the following dependencies in order to configure your environment.

[Docker](https://www.docker.com/) Install a desktop client.

[Git](https://git-scm.com/) Install a console client.

#### Installation
Open a bash console and follow the steps below:

1. Clone the scala-notebooks repository
```
https://github.com/LambdaFanatics/scala-notebooks.git scala-notebooks
```

2. Navigate to the local repository folder
```
cd scala-notebooks
```

3. Run and install the scala-jupyter docker container.
```
docker run --rm -it -d -p 8888:8888 -v <absolute-path-to-repository>/notebooks:/notebooks --name scala-jupyter  dockoey/jupyter-scala:211.jdk8
```

4. Open a browser and navigate to
```
http://localhost:8888
```

5. Upon task completion stop the container
```
docker stop scala-jupyter
```

6. Repeat steps 3 to 4 to re-run the container
