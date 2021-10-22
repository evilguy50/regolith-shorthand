filter for having shorthand syntax inside of functions.

example config:

    [define]
    shorts = admin armors

    [as]
    admin_long = @a[tag=admin]
    armors_long = @e[type=armor_stand]
    
example inside a function:

    execute admin ~ ~ ~ kill armors
    
compiles into:

    execute @a[tag=admin] ~ ~ ~ kill @e[type=armor_stand]
    
