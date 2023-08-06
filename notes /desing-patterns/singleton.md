# Patron de diseño `Singleton`.

Recuerda que puedes encontrar más información en el siguiente enlace [Refactoring Guru "Singleton".](https://refactoring.guru/es/design-patterns/singleton)

___

🔒 Descubre el patrón de diseño "Singleton": Garantizando una única instancia 🔒

El patrón de diseño "Singleton" es una joya en el mundo del desarrollo de software. 

🌟 Es un patrón creacional que nos permite asegurarnos de que una clase tenga una única instancia en todo el programa y, al mismo tiempo, proporciona un punto de acceso global para acceder a dicha instancia. ¡Veamos por qué es tan útil y poderoso! 💡

🏢 Imagina que necesitas una clase que represente una configuración global, una conexión a una base de datos o cualquier otra entidad que no deba tener múltiples instancias. Aquí es donde el patrón "Singleton" entra en acción. Garantiza que solo haya una instancia de esa clase en toda la aplicación.

🔐 La implementación del "Singleton" implica restringir la creación de nuevas instancias mediante la utilización de un constructor privado. En su lugar, proporciona un método estático que devuelve la única instancia existente o la crea si aún no existe. De esta manera, siempre se obtiene la misma instancia en cada llamada.


```java
class Singleton {

    /**
    * Instancia unica.
    *
    */
    private static instance;

    /**
    * Constructor privado
    *
    */
    private Singleton(){}

    public static Singleton getInstance() {
        if (!Singleton.instanciaUnica) {
            Singleton.instanciaUnica = new MiSingleton();
        }
        return Singleton.instanciaUnica;
    }
}

```

🚀 La utilidad del "Singleton" radica en su capacidad para proporcionar un punto de acceso global a su única instancia. Esto significa que puedes acceder a esta instancia desde cualquier lugar de tu código, lo que facilita la comunicación y el uso compartido de recursos cruciales.

¡Aprovecha el patrón de diseño "Singleton" en tus proyectos y benefíciate de la seguridad y la simplicidad que ofrece! 🚀

#SingletonPattern #DesignPatterns #CreationalPattern #SoftwareDevelopment #CodeQuality
