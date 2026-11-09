# MG5
## Devlog
1) I believe that using a NavMesh VS is more advantageous to use on 3d and realistic games that rely on set physics that are similar to our own world, including gravity and general motion
and/or direction. A game such as Skyrim, which although a fantasy game 3d adventure game, does still try to stay as grounded and realistic as it can with their npcs, and thus would rely on
a NavMesh to help support the constant rules of motion in our world, and reflect it onto the game. Alternatively, a more unrealistically motioned or 2d game may not require a NavMesh, take
Among Us, a 2d detective and callaborative game set in outer space, that has very basic movement that only needs to reflect upon the y-axis for vertical movement, and would only be stopped by invisible barriers. This game does not require all the capabilities that a NavMesh has to offer, nor would it benefit from one as it would take up extra data, so having a much more simple movement system with cartoonish physics and needs to be able to make up its own rules for this, through the exaggerated playstyle.

2) Within the loop for BirdManager, it appears the call to Vector3.Distance is being used to compare the bird's current position via "bird.transform.position", and the player's position as
"_player.position", predefined by the _player data member as a Transform variable. This number, which becomes smaller the closer the player's current position is to the bird's position, is
then compared to be less than or equal to a defined float data member labelled "_interactDistance", in which the if condition would be fulfilled if the player gets close enough. This then trigges the method of bird called "RunAway" with a parameter of the player's position, so it can likely be assumed that all birds in the _birds array that are close enough to the player to
cause the comparison in distance between the bird and player to be under _interactDistance, to then try to run away in a different direction from the player.

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [Mountain fantasy environment models](https://www.fab.com/listings/60487a72-3f20-4bb2-aa78-247ed1582656)