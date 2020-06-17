# Divy Dhiman

[Repo](https://github.com/DivyDhiman/example1)

## Things we liked
- Pull to refresh is implemented
- Your use of Android Architecture Components
  - ViewModel

## Reasons why the submission fell short

Primary reasons:
- Cannot maintain state (e.g. loaded items, scroll position of RecyclerView) after device configuration change (e.g. screen rotation)
- Use of !! in Kotlin code

Secondary reasons:
- No address displayed in delivery list
- The Espresso test dosen't verify any data displayed e.g. RecyclerView item TextViews, Map detail TextViews
- The package of test classes not match with file location
- Classes with constants only can change to object and no need to use `companion object`
- In `CentraliseCheck`, should use `applicationContext.getSystemService(Context.CONNECTIVITY_SERVICE) as? ConnectivityManager` to get ConnectivityManager

## Suggestions/Things Can Be Improved
- We found you can apply a dependency injection.
- We found you can try to use ?./lateinit var to avoid !! in Kotlin code
- We found you can add more files in .gitignore
- We found you can use Kotlin `data class` to write `MockList`. And use `@Parcelize`, so it can be parse between Activities.