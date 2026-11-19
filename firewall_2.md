### @explicitHints 1
### @flyoutOnly true

# Anomalía 1

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
})

```

## Anomalía 1 @showdialog
¡Son anomalías! Esta anomalía parece tener muchas patas y está intentando entrar en el castillo...   
¡Tenemos que crear una regla para que no entre!   
![Anomalía](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_2.jpg)


## Regla de denegar
Tenemos que pensar una regla que impida el paso a la anomalía, pero que siga dejando entrar a los aldeanos.   
Añade un bloque ``||cyber:Añadir regla de denegar||`` a tus reglas. Sirve para decirles a los guardias que no dejen pasar a nada que cumpla la regla.  

### Rasgos que los diferencian
¿Ves algo que nos ayude a distinguir entre un aldeano y esta anomalía?   
Si no lo tienes claro, pulsa el botón < (atrás) para volver a mirar desde el puesto de vigilancia qué se acerca.
```template
cyber.setupFirewall(function () {
cyber.allowAll()
})
```

### ~ tutorialhint
```blocks
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
})

```

```package
minecraft-ciberseguridad-es=github:avilesalexmj-dev/minecraft-ciberseguridad-es
```
