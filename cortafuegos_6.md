### @explicitHints 1
### @flyoutOnly true

# Soldados

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
    cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireLegs(Legs.OverFourLegs), cyber.requireHoldingItem(HoldingItem.NoItem)))
    cyber.addDenyFirewallRule(cyber.requireEyewear(WearingEyeware.WearingEyeware))
    cyber.addDenyFirewallRule(cyber.requireCrest(cyber.createGridString(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)))
})

```

## Soldados @showdialog
Parece que al reino rival no le ha sentado nada bien que bloqueemos a sus espías, ¡y ha enviado soldados!   
![Soldados](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_6.jpg)


## ¡Soldados!
¡Rápido, crea reglas para bloquear a estos soldados! ¡No podemos dejar que crucen las murallas del castillo!   
Podríamos fijarnos en el escudo real que llevan pintado para distinguirlos. Nuestros soldados llevan un escudo **dorado** y **morado**, y a ellos sí hay que dejarles volver a entrar.   


```template
cyber.setupFirewall(function () {
cyber.allowAll()
cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireHat(WearingHat.NoHat), cyber.requireHoldingItem(HoldingItem.NoItem)))
cyber.addDenyFirewallRule(cyber.requireEyewear(WearingEyeware.WearingEyeware))
})
```

### ~ tutorialhint
Fíjate bien en los escudos de los soldados. ¿Podríamos filtrar por ellos? ¡Pero cuidado con no bloquear a nuestros soldados!
![Escudos de los soldados](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_6_shields.jpg)



```package
bloques-ciberseguridad-es=github:avilesalexmj-dev/pxt-ciberseguridad-es
```
