### @explicitHints 1
### @flyoutOnly true

# Combinar reglas

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
    cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireLegs(Legs.OverFourLegs), cyber.requireHoldingItem(HoldingItem.NoItem)))
})

```

## Más aldeanos @showdialog
Parece que se acerca un grupo grande de aldeanos.   
¿Les dejará pasar a todos el cortafuegos?   
![Aldeanos](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_4.jpg)


## Más aldeanos
Puede que necesites crear reglas con una **y**. Así puedes combinar 2 reglas en una.   
Cuidado: algunos de estos aldeanos no llevan sombrero, pero llevan objetos como un pico o un mapa. Por eso no podemos bloquear sin más a todo el que no lleve sombrero.  


```template
cyber.setupFirewall(function () {
cyber.allowAll()
cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
})
```

### ~ tutorialhint
Parece que la anomalía no lleva sombrero y tampoco lleva nada en la mano.

```package
bloques-ciberseguridad-es=github:avilesalexmj-dev/pxt-ciberseguridad-es
```
