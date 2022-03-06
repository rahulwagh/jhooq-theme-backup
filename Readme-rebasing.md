## Add remote upstream repo which hugo-clarity

```
git remote add upstream https://github.com/chipzoller/hugo-clarity.git   
```

## Fetch all the branches of that remote into remote-tracking branches, such as upstream/master:

```
git fetch upstream
```

## rebase your branch
```
git rebase upstream/master
```

## git clone recursively 
```
git clone --recurse-submodules https://github.com/chipzoller/hugo-clarity.git
```

## how i added  a submodule

1. Goto `.gitmodules` and update the following content 

```
[submodule "themes/jhooq-theme"]
	path = themes/jhooq-theme
	url = https://github.com/rahulwagh/jhooq-theme.git
```

2. Goto `config.toml` update the theme path

```
theme = "jhooq-theme"
```

## how to take update of submodule

Goto the directory `themes/jhooq-theme` and then run the normal 

```
git pull https://github.com/rahulwagh/jhooq-theme
```

it will update your submodule