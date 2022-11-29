<img src="https://siceuc2.ucol.mx/becatitulaciongobiernodelestado/Assets/images/03UdeC_publi_80.png">

# Universidad de Colima 
## Facultad de Ingeniería Mecánica y Eléctrica 
### "Ingenieria en Computacion Inteligente"
### Alumno:
  * Jason Humberto Garcia Camacho 
### Maestro:
  *  Walter Alexander Mata Lopez
--------------------------------------------------
# Portafolio De Programas Relalizados En La tercera Parcial En Lenguage de Elixir


---------------------------------------------------

## Case

Ejemplo 1


    defmodule Persona3 do
      def sexo(sex) do
        case sex do
           :m -> "Masculino"
           :f -> "Femenino"
            _ -> "Sexo desconocido"
           end
          end
         end
    
----------------------------------------------------
## Match con funciones

Ejemplo 1

    defmodule Persona4 do
     def sexo(sex) when sex == :m do
        "Masculino"
     end
     def sexo(sex) when sex == :f do
        "Femenino"
     end
     def sexo(_sex) do
       "sexo desconocido"
     end
    end
    

Ejemplo 2 


    defmodule Persona5 do
      def sexo(sex) when sex == :m, do: "Masculino"
      def sexo(sex) when sex == :f, do: "Femenino"
      def sexo(_sex), do: "sexo desconocido"
    end
    
--------------------------------------------------------------

## cond

Ejemplo 1 

     defmodule Persona6 do
       def sexo(sex) do
        cond do
         sex == :m -> "Masculino"
         sex == :f -> "Femenino"
         true -> "Sexo desconocido"
        end
       end
     end

   
---------------------------------------------------------------
## Herramienta mix 

crear un proyectos desde la terminal

comando ingresado en la terminal:

     mix new calculadora
     
### Carga de una aplicación 

Ingresar al directorio dondese creo la nueva aplicación 

      C:\>cd calculadora
  
Asi se ve cuando lo hiciste bien 

      C:\calculadora>

Lanzar el shell de Elixir con mix 
     
      iex -S mix
      
Asi se ve cuando lo hiciste bien 
  
      C:\calculadora>iex -S mix
      Compiling 1 file (.ex)
      Generated calculadora app
      Interactive Elixir (1.10.4) - press Ctrl+C to exit (type h() ENTER for help)
      iex(1)>
      
Ejecutar la función hello() 
        
      iex(1)> Calculadora.hello()
      :world
      iex(2)>

### Documentación con ExDoc 

Abrir el archivo mix.exs
Modificar las dependencias agregando {:ex_doc, “~>0.12”} 

      defp deps do
          [
            {:ex_doc, "~>0.12"}
          ]
      end
      
 Ejecutar el comando mix deps.get
 
      C:\calculadora>mix deps.get
      
Asi se ve cuando lo hiciste bien 

      Resolving Hex dependencies...
      Dependency resolution completed:
      New:
      earmark_parser 1.4.12
      ex_doc 0.23.0
      makeup 1.0.5
      makeup_elixir 0.15.0
      nimble_parsec 1.1.0
      * Getting ex_doc (Hex package)
      * Getting earmark_parser (Hex package)
      * Getting makeup_elixir (Hex package)
      * Getting makeup (Hex package)
      * Getting nimble_parsec (Hex package)
 
 
