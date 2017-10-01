# Space-Simulator-2k18
After completing the C++ book I bought, I seek to apply this knowledge in a text-based space exploration game.

In Space Cowboy Simulator 2k18, I want to create an array of Planet objects that are randomly generated. This is the first step, and it's the step I can't get past already, auauau. In the Planet type constructor, I have it randomly set an m_Type variable to 'A'-'E' or ' ', the idea being the when I create an array of these Planet types to represent a map, it will have Planet objects with a random assortment of m_Type values. This isn't working, however, as all the Planet type objects in the array are being instantiated with the value of m_Type set to ' '.

My questions: How do I fix this? Why is this happening? I assume it's one of two causes:
  1. When it's filling the array, it's instantiating a single Planet object and then a bunch of copies of it.
  2. The Planet objects are instantiated at the same time, causing the "random" number to be the same, but aren't copies of one object.
