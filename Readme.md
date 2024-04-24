# Simple Flask CD pipeline 

1. Set up GitHub Account & Repo

2. Set up DockerHub account

# Set up python environment called env
3. python3 -m venv env

# Activate virtual environment env
4. source env/bin/activate

# Install Flask
5. pip install flask

# Generate requirements.txt
6. pip freeze > requirements.txt

# Run the app locally
6. python3 app.py

7. Add your `DOCKER_USERNAME`, `DOCKER_PASSWORD`, `DOCKERHUB_REPO` at Github -> Settings -> Secrets and variables -> Actions

8. GitHub-> Repo -> Action -> `Publish Python package` -> `Set up this workflow`

9. Paste contents of python-publish.yml

10. `Start commit`

11. GitHub Repo -> Paste contents of cd_config.yml to workflow description field

12. git add . && git commit -m"added app code" && git push

13. Navigate to DockerHub & discover your freshly built & served image of Flask App!




Detailed instructions:
https://www.section.io/engineering-education/ci-cd-pipelines-with-flask-docker-and-github-actions/