# sliver_experience

A new Flutter project.

## Getting Started

This is a sliver example project. It can be reach from https://www.youtube.com/live/YY-_yrZdjGc?feature=share

A sliver is a portion of a scrollable area, which means anything that scrolls in Flutter is a sliver. ListView and GridView are a kind of sliver.

When we wrap the Column in a SingleChildScrollView, we’re essentially wrapping the Column in a sliver. Slivers lay out using SliverContraints and have a SliverGeometry. When you work with slivers, the window size that we were constricted to previously becomes an infinite amount of space in the given axis. So, we use language different from height, width, and position. For a sliver, we need to know things like how much is visible, how far to the next sliver, and how far we scrolled. The answers enable us to lazily load slivers, meaning we only build slivers that we can see and a little bit of the ones on either edge. This makes scrolling more efficient because we won’t build slivers that we don’t need because the slivers aren’t seen.

A floating SliverAppBar will scroll out of view, but it scrolls back into view when the user scrolls back in that direction, regardless of the current position in the scroll view.

We can fill the expandedHeight of our app bar, for an even more dynamic UI. We can do this with the FlexibleSpaceBar. This widget is designed to stretch and collapse its content. 
