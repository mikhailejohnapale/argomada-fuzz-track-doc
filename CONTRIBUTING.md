# Contribution Instructions

## 1. Fork the repository
1. Open in a new tab [https://github.com/argomada/argomada-fuzz-track-doc](https://github.com/argomada/argomada-fuzz-track-doc)
2. In the top-right corner of the page, click the Fork button.

## 2. Clone the forked repository
1. On GitHub, navigate to your fork.
2. In the right side of your fork's repository page, copy the clone URL.
3. Open a terminal, copy and paste the commands below and hit enter.
4. Rename `username` below to your github username.

```
cd ~/Downloads
git clone git@github.com:username/argomada-fuzz-track-doc.git
cd base-repo
```

## 3. Set upstream URL
Open a terminal, copy and paste the command below and hit enter.

```
git remote add upstream git@github.com:argomada/argomada-fuzz-track-doc.git
```

## 4. Create a feature branch
Open a terminal, copy and paste the command below and hit enter.

```
git checkout -b branch-name
```

## 5. Make your contribution in the feature branch

```
echo "make your changes"
```

## 6. Check for changes
Open a terminal, copy and paste the commands below and hit enter.

```
# if any file(s) is added
git status
# changes inside the files
git diff
```

## 7. Commit your changes
Open a terminal, copy and paste the command below and hit enter.
Please make messages that describe your work.

```
git commit -am "contribution description"
```

## 8. Pull new commits from upstream
Open a terminal, copy and paste the command below and hit enter.

```
git pull upstream master
```

## 9. Push your changes to your remote repository
Open a terminal, copy and paste the command below and hit enter.

```
git push origin branch-name
```

## 10. Create a pull request.
1. Navigate to your repository.
2. Switch to your feature branch.
3. Click the compare & review button.
4. Review the pull request.
5. Press create pull request button.
