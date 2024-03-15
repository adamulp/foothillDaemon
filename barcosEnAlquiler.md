```mermaid
classDiagram
    class Alquier{
        - String nombre
        - Double dni
        - LocalDate fechaAlquiler
        - LocalDate fechaDevolución
        - int amarre
        - Barco alquilado
    }

    class Barco {
        - String matricula
        - int eslora
        - LocalDate fabricación
    }
    Alquileres o-- Alquiler
    Alquiler <-- Barco


    class Yate{
        - Double potenciaCV
        - int camarotes
    }

    class BarcoMotorizado{
        - double potenciaCV

    }

    class Velero{
        -int mastiles

    }

    Barco <|-- BarcoMotorizado
    BarcoMotorizado <|-- Yate
    Barco <|-- Velero

//Hi Adam,good work..
}
