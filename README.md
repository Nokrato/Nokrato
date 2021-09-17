```kotlin
class Centauri07: Profile("Andrei John", 14, SimpleDateFormat("MM-dd-yyyy").parse("01-02-2007")) {
    init {
        addHobby("Programming", "Playing Guitar")
        addLanguage("Java", "Kotlin")
    }
}
```

```kotlin
abstract class Profile(val name: String, val age: Int, val birthDate: Date) {
    val hobbies: MutableList<String> = mutableListOf()
    val languages: MutableList<String> = mutableListOf()

    fun addHobby(vararg hobbies: String) {
        this.hobbies.addAll(*hobbies)
    }
    
    fun addLanguage(vararg languages: String) {
        this.languages.addAll(*languages)
    }
}
```

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=Centauri07&theme=prussian&show_icons=true)
