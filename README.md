# SimuladorFidelizacion
Algoritmo SimuladorFidelizacion
    Definir total, precioProducto Como Real
    Definir continuar Como Cadena
    
    total <- 0
    continuar <- "s"
    
    Escribir " CARRITO DE COMPRAS CON FIDELIZACIÓN "
    
    Mientras continuar = "s" O continuar = "S" Hacer
        Escribir "Ingrese precio del producto: $"
        Leer precioProducto
        
        Si precioProducto > 0 Entonces
            total <- total + precioProducto
            Escribir "Producto agregado. Total parcial: $", total
        Sino
            Escribir "Precio inválido, no se agregó el producto."
        FinSi
        
        Escribir "¿Agregar otro producto? (s/n):"
        Leer continuar
    FinMientras
    
    Escribir " TOTAL DE COMPRA "
    Escribir "Monto acumulado: $", total
    
    
    Si total > 500 Entonces
        total <- total * 0.85  
        Escribir "¡Descuento VIP del 15% aplicado!"
        Escribir "Total con descuento: $", total
    Sino
        Escribir "No aplica descuento VIP (mínimo $501)."
    FinSi
    
    Escribir "Gracias por su compra."
	
FinAlgoritmo
