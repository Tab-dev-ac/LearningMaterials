Tilemap collider 2D
Composite collider 2D
rigidbody 2D (body type: static)

Unity APIs: https://docs.unity3d.com/ScriptReference/Input.GetKey.html

Chapter and Contents
1.
34. Polish
+ UI constraints
+ If fall then reset the level
+ disable user control when character touch the cliff
+ Eliminate the small gap between sprite blocks (Change bg grid size)
+ make the frog not moving after death
```
 (rb.bodyType = RigidbodyType2D.Kinematic)
GetCompnent<Collider2D>().enabled = false;
```
35:GUI upgrade

