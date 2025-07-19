# Programa_estruturado
En una empresa de logistica, requiere un software, donde se pueda calcular el coste de las entregas.
# Programa para empresa de logística
def calcular_costo(distancia, tiempo):
    return (distancia * 0.5) + (tiempo * 10)
# funcion 
def main():
    # Solicitar datos al usuario
    distancia = float(input("Ingresa la distancia a recorrer (km): "))
    tiempo = float(input("Ingresa el tiempo estimado (horas): "))
    capacidad_carga = float(input("Ingresa la capacidad de carga (kg): "))
# Calcular costo de entrega
    costo = calcular_costo(distancia, tiempo)

# Evaluar si la carga es aceptable
    if capacidad_carga > 1000:
        print("La carga excede la capacidad máxima.")
    else:
        print(f"Costo de entrega: {costo:.2f} unidades monetarias")

# Ejecutar la función principal
if __name__ == "__main__":
    main()
