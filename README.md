# eFurry Android Translation
Translation files for the eFur Android app

## How to translate
The source (English) file is located at [app/src/main/res/values/strings.xml](app/src/main/res/values/strings.xml).

The easiest way to translate is to create a new Android Studio project and import all the xml files in the `values` directory and use the [Translations editor](https://developer.android.com/studio/write/translations-editor).

### Translate into a new language
Create a folder in `app/src/main/res/` named `values-XX`, where `XX` is the two-letter ISO 639-1 country code for the target language. E.g. for French the folder would be named `values-fr`.

Inside this folder create a file `strings.xml` (so the full path would be `app/src/main/res/values-fr/strings.xml`) with the following content:

```
<resources>
</resources>
```

A Github Action will be started that automatically translates the source file into the target language. Check the progress in the [Actions](https://github.com/eFurry/android-translation/actions) tab.

Alternatively, copy lines from the source file and translate one at a time manually.

### Update an existing translation
Locate the language you want to translate in the [app/src/main/res/](app/src/main/res/) directory. E.g. for Spanish it is the file `values-es/strings.xml`.

Fork the repository and open a pull request with your changes!
