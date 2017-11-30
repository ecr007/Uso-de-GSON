# Uso-de-GSON

```

String json = "{\"nombre\":\"Unai\",\"edad\":28}";

    Gson gson = new Gson();

    Persona persona = (Persona) gson.fromJson(json, Persona.class);    

    System.out.println(persona.getNombre());
    System.out.println(persona.getEdad());
    
    
    ```
