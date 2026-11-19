### @explicitHints 1
### @flyoutOnly true

# Permitir todo

## ¿Qué es un cortafuegos? @unplugged
Un cortafuegos (firewall) es un sistema que filtra el tráfico que entra (y a veces el que sale) de una red o de un lugar.   
Funciona con reglas que permiten o deniegan distintos tipos de tráfico.   
En esta tarea vas a crear una serie de reglas para dejar entrar en el castillo a unos personajes y a otros no.

## Aldeanos @unplugged
Parece que se acerca un grupo de aldeanos. Deberíamos dejarlos entrar en el castillo. Empecemos creando un cortafuegos que lo permita todo.   
![Aldeanos](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_1.jpg)
## Paso 1
Se acerca un grupo de aldeanos. Empecemos creando un cortafuegos que lo permita todo.   
Cuando quieras probar el cortafuegos, pulsa el botón de reproducir (▶).
```template
cyber.setupFirewall(function () {
})
```

### ~ tutorialhint
```blocks
cyber.setupFirewall(function () {
    cyber.allowAll()
})

```

```package
ciberseguridad-es=github:avilesalexmj-dev/minecraft-ciberseguridad-es
```
