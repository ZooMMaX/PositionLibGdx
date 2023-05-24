# PositionLibGdx

![Maven Central](https://img.shields.io/maven-central/v/ru.zoommax/PositionLibGdx?color=00ff)

### Dependency
![dependency maven](https://img.shields.io/badge/DEPENDENCY-Maven-C71A36?style=plastic&logo=apachemaven)
```xml
<dependencies>
    <dependency>
        <groupId>ru.zoommax</groupId>
        <artifactId>PositionLibGdx</artifactId>
        <version>1.0</version>
    </dependency>
</dependencies>
```

![dependency gradle](https://img.shields.io/badge/DEPENDENCY-Gradle-02303A?style=plastic&logo=gradle)
```groovy
implementation 'ru.zoommax:PositionLibGdx:1.0'
```

### Set position

```java
import ru.zoommax.position.Percent;
import ru.zoommax.position.SIDE;
import com.badlogic.gdx.scenes.scene2d.Actor;

public class Main {
    public static void main(String[] args) {
        
        Actor a = new Actor();
        Actor b = new Actor();
        
        Percent.size(a, 10, 10);
        Percent.pos(a, SIDE.PARENTBOTTOMRIGHT);
        Percent.size(b, 20, 10);
        Percent.pos(b, SIDE.RIGHTofLEFT, a);
    }
}
```