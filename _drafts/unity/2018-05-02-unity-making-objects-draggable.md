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
		Vector3 pos = Camera.main.ScreenToWorldPoint(Input.mousePosition);
		pos.z = 0;
		gameObject.transform.position = pos;
	}
}
{% endhighlight %}