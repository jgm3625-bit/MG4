# MG4
## Devlog
There is _up variable that is set as bool, because we would set true and false to determine whether it moves up or down. There is a _timer variable as a float to count down the seconds in decimal until it changes direction. Now, Start() is when the game runs the _timer = _switchSpeed, which means it counts down for 3 seconds, because _switchSpeed = 3.0f. Then, it Update() to run every frame on _up would move up or down as true (_moveSpeed * Time.deltaTime) or false (-_moveSpeed * Time.deltaTime) within those values. It would countdown for 3 seconds, because of _timer -= Time.deltaTime. Now from there, if _timer is less than 0, it would reset to _switchSpeed (_timer = _switchSpeed). And it flips _up due to _up = !_up, which reverse the true and false statement in _up. With all that, it repeats every frame, because of Update(). 

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [City 3D models](https://assetstore.unity.com/packages/3d/environments/simplepoly-city-low-poly-assets-58899)
- [Bite sound effect](https://freesound.org/people/Jofae/sounds/353067/)