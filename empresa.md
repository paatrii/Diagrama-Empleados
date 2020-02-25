classDiagram

      Empresa <|-- Empleado
      Directivo <|-- Empleado
      Empresa <|-- Cliente
      Empleado <|-- Directivo

      class Empleado{
         -SueldoBruto : Integer
         -nombre : String 
         -edad : Integer
         +calcular_salario_neto()void
         +mostrar() void
      }

      class Cliente{
         -telefono : String
         -nombre : String
         -edad : Integer
         +mostrar() void
      }

         class Empresa{
          -nombre : String
          -Cif : String

      }
      class Directivo{
         -categoria : String
         -empleados_subordinados()
         +mostrar()
      }
```