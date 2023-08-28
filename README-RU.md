# Core JS 101 (Stage 0 Version)

:warning: **Обратите внимание, что нельзя открывать PR, содержащие ответы на этот репозиторий!**

Однако, PRs с исправлениями или предложениями приветствуются!

## Task
Задача — реализовать функции по разным тематикам Core JS. Всего восемь модулей с разными задачами. Каждый модуль состоит из заданий по заданной теме:

1. Strings
2. Numbers
3. Arrays
4. Conditions and Loops

**Активное использование [documentation](https://developer.mozilla.org/en-US/) настоятельно рекомендуется!**

## Prepare and test
1. Установите Node.js
2. Форкнуть этот репозиторий: https://github.com/Luffi2539/core-js-101/
3. Клонируйте только что созданный репозиторий: `https://github.com/<%your_github_username%>/core-js-101/`
4. Перейти в папку `core-js-101`
5. Для установки всех зависимостей используйте `npm install`
6. Каждая задача обычно представляет собой обычную функцию:
    ```javascript
      /**
       * Returns the result of concatenation of two strings.
      *
      * @param {string} value1
      * @param {string} value2
      * @return {string}
      *
      * @example
      *   'aa', 'bb' => 'aabb'
      *   'aa',''    => 'aa'
      *   '',  'bb'  => 'bb'
      */
      function concatenateStrings(value1, value2) {
        throw new Error('Not implemented');
      }
    ```
   Описание задачи читайте в комментарии над функцией. Попытайтесь понять идею. Вы можете увидеть подготовленные тесты, если вы их не понимаете.
7. Напишите свой код в `src/*.js`.

   Удалите строку ошибки выдачи из тела функции:
    ```javascript
        throw new Error('Not implemented'); 
    ```
   Реализуйте функцию любым способом и проверьте свое решение, выполняя тесты до тех пор, пока непройденный тест не станет пройденным (зеленый).
8. Запустите `npm test` в командной строке. Если все в порядке, можно попробовать решить следующую задачу.

## Submit to [rs app](https://app.rs.school/)
1. Open [rs app](https://app.rs.school/) and login
2. Go to Auto-test
3. Select your task (Core JS 101)
4. Press submit button and enjoy

## Notes
* We recommend you to use nodejs of version 16 or lower. If you using any of features that does not supported by node `v16`, score won't be submitted.
* Please be sure that each of your test in limit of 30sec.
* You will get 0 (zero) if you have any eslint's errors or warnings.

## FAQ
**Question:** I use Windows machine and have received a lot of errors like "Expected linebreaks to be 'LF' but found 'CRLF'". How to handle it?

**Answer**:
- First, you need to install Gitbash properly: you need to choose option "Checkout as-is, commit as-is" in section "Configuring the line ending conversions". It'll let you download repos with line endings set "as-is" as well as commit. In other words, not to change them at all, because by default it converts them.
- Second, install `editorconfig` plugin to your editor. For VS Code you can find it here:
https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig

  I'll let you apply some rules when you saving your files in the repo. This plugin will use config-file `.editorconfig` that you can see in the root folder. It lets you save the file with needed line endings, trim whitespaces, etc.
- Finally, you need to apply linter's autofix feature in order to fix all linebreaks that was already changed to "CLRF":
```
$ npm run lint -- --fix
``` 

___
The task based on https://github.com/rolling-scopes-school/js-assignments.
