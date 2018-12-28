#Useful Commands -

**Build the images:**
```docker-compose -f docker-compose-dev.yml build```

**Run the containers:**
```docker-compose -f docker-compose-dev.yml up -d```

**Create the database:**
```docker-compose -f docker-compose-dev.yml run users python manage.py recreate_db```

**Seed the database:**
```docker-compose -f docker-compose-dev.yml run users python manage.py seed_db```

**Run the tests:**
```docker-compose -f docker-compose-dev.yml run users python manage.py test```

**Run the tests with Coverage:**
```docker-compose -f docker-compose-dev.yml run users python manage.py cov```

**Code Linting:**
```docker-compose -f docker-compose-dev.yml run users flake8 project```

**To stop the containers:**
```docker-compose -f docker-compose-dev.yml stop```

**To bring down the containers:**
```docker-compose -f docker-compose-dev.yml down```

**Want to force a build?**
```docker-compose -f docker-compose-dev.yml build --no-cache```

**Remove images:**
```docker rmi $(docker images -q)```

**Access postgres database:**
```docker-compose -f docker-compose-dev.yml exec users-db psql -U postgres```


# Microservices with Docker, Flask, and React

[![Build Status](https://travis-ci.org/YOUR_GITHUB_USERNAME/testdriven-app.svg?branch=master)](https://travis-ci.org/palasgaonkar/testdriven-app)
