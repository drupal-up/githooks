#### 0. Have a setup with composer with a the web folder not in the root folder and install code sniffer with
```
composer --global require drupal/coder
```
#### 1. Have a .githooks folder with executables
```
chmod -R 777 .githooks
```
#### 2. Run
```
git config core.hooksPath .githooks
```
#### 3. Make sure you have a pre-commit script .githooks/pre-commit

#### 4. Make sure it is executable.
```
chmod +x .githooks/pre-commit
```
#### 5. Voila. Next time you try to commit some code - code sniffer will check for Drupal Standards and best practices.
