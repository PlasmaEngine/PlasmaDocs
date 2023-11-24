 `Event` `Physics`



(NOTE) Information about a collision in physics. Sent when collisions start, persist, or end.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ FirstPoint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/collisionevent.markdown#firstpoint-plasma-engine-d)|[basecollisionevent](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/basecollisionevent.markdown)| |


 #  Properties


---  
 #  FirstPoint : [contactpoint](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/class_reference/contactpoint.markdown)

 `read-only`

> Convenience function to return the first ContactPoint. Some logic only cares about one point of information. In a more general case all points should be iterated over.
> ``` lang=cpp, name=Lightning
> var FirstPoint : ContactPoint


---  
 #  Methods


---  
 

 