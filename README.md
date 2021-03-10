# Uso-de-GSON

```java

// Class

public class Persona implements Serializable {
    private String nombre;
    private int edad;

    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public int getEdad() {
        return edad;
    }

    public void setEdad(int edad) {
        this.edad = edad;
    }
}

// To Json
Persona persona = new Persona();
persona.setNombre("Unai");
persona.setEdad(28);

Gson gson = new Gson();        
System.out.println(gson.toJson(persona));

// From Json
String json = "{\"nombre\":\"Unai\",\"edad\":28}";

Gson gson = new Gson();

Persona persona = (Persona) gson.fromJson(json, Persona.class);    

System.out.println(persona.getNombre());
System.out.println(persona.getEdad());
```
