---
layout: post
title:  "Unity - Making Objects Draggable"
categories: unity
---

Recently I have started to develop on the gaming platform, Unity. And I have
loved working with it. You can easily (well at least I do) create games using
the Unity3D editor, then attach scripts written in either C# or Javascript to
make your games work.

So, in one of my current projects, I am working on a physics puzzle game when
the aim is to get 3 balls into the 3 goals, using limited balls. The twist is,
there are certain objects that you can drag around the field to help you finish
the level.

Attaching this little script to an object will allow it to be draggable with a
mouse or touch input.

{% highlight c# %}
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Draggable : MonoBehaviour {
	private void OnMouseDrag() {
		// Converts the touch or click position into a position in the world
		Vector3 pos = Camera.main.ScreenToWorldPoint(Input.mousePosition);

		// Zeros the z-axis as I am working on a 2D game
		pos.z = 0;

		// Move the GameObject to that position
		gameObject.transform.position = pos;
	}
}
{% endhighlight %}

Hope this is helpful

Nilo 