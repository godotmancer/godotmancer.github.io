# Introduction


Some *GDScript* code to test highlighting.

<!--more-->


# This is a new post from HUGO

```gdscript
extends Spatial

onready var camera := $Camera
onready var cube := $CubeSimple
onready var ships_container := $ShipsContainer

var perform_raycast : bool = false
var ray_from : Vector3 = Vector3.ZERO
var ray_to : Vector3 = Vector3.ZERO
var path = []

# Called when the node enters the scene tree for the first time.
func _ready() -> void:
	Signals.connect_to_all_cubes_depleted(self, "_all_cubes_depleted")
	cube.color = Utils.get_noice_random_color()

```

## Some quotes...

A quote by any other...

> This is one of the most awesomest game engine on the planet

### A Logo...

![Logo](/img/godotmancer-logo.jpg "The Mancer")
