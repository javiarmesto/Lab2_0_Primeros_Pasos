# Ejemplos de Prompts para AL con GitHub Copilot

## Ejemplo 1: Crear un Campo en una Tabla
**Prompt:**
"Crea un campo en AL para almacenar los puntos de un cliente con validación."

**Resultado:**
```al
tableextension 50100 "Customer Points Extension" extends "Customer"
{
    fields
    {
        field(50000; "Customer Points"; Integer)
        {
            DataClassification = CustomerContent;
            Caption = 'Customer Points';
        }
    }
}
```

## Ejemplo 2: Extender una Página
**Prompt:**
"Extiende la página de clientes para mostrar el campo de puntos."

**Resultado:**
```al
pageextension 50101 "Customer Points Extension" extends "Customer Card"
{
    layout
    {
        addlast(Content)
        {
            field("Customer Points"; "Customer Points")
            {
                ApplicationArea = All;
                Caption = 'Points';
                ToolTip = 'Enter the customer\'s points.';
                trigger OnValidate()
                begin
                    if "Customer Points" < 0 then
                        Error('Points cannot be negative.');
                end;
            }
        }
    }
}
```

## Ejemplo 3: Validación de Datos
**Prompt:**
"Añade validación para un campo de puntos en una tabla."

**Resultado:**
```al
trigger OnValidate()
begin
    if "Customer Points" < 0 then
        Error('Points cannot be negative.');
end;
```

## Ejemplo 4: Uso de Labels
**Prompt:**
"Usa labels para los mensajes de error."

**Resultado:**
```al
labels
{
    LabelPointsValidationError = 'Points cannot be negative.', Comment = 'Ensure points are non-negative.', Locked = false, MaxLength = 50;
}
```

## Ejemplo 5: Configuración Inicial
**Prompt:**
"Configura un proyecto AL con reglas de estilo específicas."

**Resultado:**
- Usa IDs de campo a partir de 50000.
- Incluye `DataClassification` en todos los campos.
- Usa nombres descriptivos para los campos con comillas.
- Añade la propiedad `Caption`.
- Usa `Labels` para los mensajes de error con parámetros opcionales como `Comment`, `Locked` y `MaxLength`.

---

Estos ejemplos están diseñados para ayudarte a interactuar con GitHub Copilot en proyectos AL. ¡Explora y experimenta con los prompts!
