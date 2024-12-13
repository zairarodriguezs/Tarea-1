def division_lista_enteros(lista):
    """
    Divide una lista de enteros en dos listas: una de números negativos y otra de positivos.
    Ambas listas estarán ordenadas ascendentemente.

    param lista: Lista de enteros.
    return: Tupla con dos listas: (negativos, positivos).
    """
    negativos = sorted([num for num in lista if num < 0])
    positivos = sorted([num for num in lista if num > 0])
    return negativos, positivos
lista = [ 1,-3, 5, 7,-8]
negativos, positivos = division_lista_enteros(lista)
print("Negativos:", negativos)
print("Positivos:", positivos)
