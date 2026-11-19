### @explicitHints 1
### @flyoutOnly true

# Anomalía 2

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
})

```

## Anomalía 2 @showdialog
¡Es otra anomalía!   
![Anomalía](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_3.jpg)


## Detén la anomalía
¡Esta anomalía es distinta! Añade otra regla para detener a esta anomalía en concreto.   
¿Ves algo que nos ayude a distinguir entre un aldeano y la anomalía?   
Recuerda que puedes pulsar el botón < (atrás) para volver a mirar desde el puesto de vigilancia.


```template
cyber.setupFirewall(function () {
cyber.allowAll()
cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
})
```

### ~ tutorialhint
¿Esos aldeanos llevan sombrero?


```package
bloques-ciberseguridad-es=github:avilesalexmj-dev/pxt-ciberseguridad-es
```
