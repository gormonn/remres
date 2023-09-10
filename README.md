# remres
A library or set of methods to resist DOM removal

# Motivation

Let's say you have developed a b2b widget that you distribute for shareware. By agreement, the client can use the widget utterly free of charge while the watermark is displayed. If the client pays to use the widget, there is no watermark.

And so, at some point, you discover unreliable users trying to remove or hide the watermark programmatically.

One day, I had a technical interview for the position of front-end engineer, during which I was asked an interesting, non-trivial question. How can we technically solve this problem when some of our clients are trying to hide our Watermark?

I think it all depends on the “method” of removal.

We can:
- Remove the element from the DOM.
- Hide an element using styles.

To do this, we need:
- Find the given element in the DOM.

So, there are many ways to make the removal task more difficult. E.g. MutationObserver
