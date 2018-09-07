This repository contains our fork of Airflow, which we use to make some tweaks.

To sync changes from the upstream (original) Airflow repository, run the following:

Add the upstream repo as a remote. You only need to do this once.
`git remote add upstream git@github.com:apache/incubator-airflow.git`
`git remote -v`

You should see something like this:
```
origin	git@github.com:All-Turtles/incubator-airflow.git (fetch)
origin	git@github.com:All-Turtles/incubator-airflow.git (push)
upstream	git@github.com:apache/incubator-airflow.git (fetch)
upstream	git@github.com:apache/incubator-airflow.git (push)
```

Fetch changes from the upstream and merge them.
```
git fetch upstream
git checkout master
git merge upstream/master
git push
git push --tags
```
