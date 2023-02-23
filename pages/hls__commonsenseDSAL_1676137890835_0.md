file:: [commonsenseDSAL_1676137890835_0.pdf](../assets/commonsenseDSAL_1676137890835_0.pdf)
file-path:: ../assets/commonsenseDSAL_1676137890835_0.pdf

- efficiency
  ls-type:: annotation
  hl-page:: 22
  hl-color:: yellow
  id:: 63f77bd5-4fb0-458b-a636-ca7451e0c99f
- high-quality code
  ls-type:: annotation
  hl-page:: 22
  hl-color:: yellow
  id:: 63f77bf5-2f47-4174-93b7-fb9454a6627a
- Maintainability
  ls-type:: annotation
  hl-page:: 22
  hl-color:: yellow
  id:: 63f77bfb-e1d9-4bd7-9a99-d3255f120baa
- readability, organization, and modularity of one’s code
  ls-type:: annotation
  hl-page:: 22
  hl-color:: yellow
  id:: 63f77bfd-4bc7-445c-955c-087f06108fcb
- Data structures refer to how data is organized
  ls-type:: annotation
  hl-page:: 23
  hl-color:: yellow
  id:: 63f77c2d-f65d-4c6d-b3dd-bf8c49e3e4d3
- Depending on how you choose to organize your data, your program may run faster or slower by orders of magnitude.
  ls-type:: annotation
  hl-page:: 24
  hl-color:: yellow
  id:: 63f77c53-c827-4074-8c55-c0de79192419
- thousands of people simultaneously, the data structures you select may affect whether your software runs at all, or simply conks out because it can’t handle the load.
  ls-type:: annotation
  hl-page:: 24
  hl-color:: yellow
  id:: 63f77c6d-e56d-4cc8-a1e2-d086dbf9b761
- The Array: The Foundational Data Structure
  ls-type:: annotation
  hl-page:: 24
  hl-color:: yellow
  id:: 63f77c86-9047-4506-b8c2-8352d3417e45
- Read: 
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 63f77cc6-574c-463e-939c-e9fb76ca8cb1
- Search: S
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 63f77cc8-358a-422c-bb24-6991e1addeae
- Insert:
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 63f77cc9-509e-45ab-bbdb-0a082044d14c
- Delete: 
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 63f77ccb-5b0a-4f33-843f-3cac32c39de8
- With an array, this means looking up a value at a particular index.
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 63f77ce5-05d0-4f57-8d12-30358e075c37
- With an array, this means looking to see if a particular value exists within the array, and if so, at which index.
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 63f77ced-61b6-4649-845b-099e23f09153
- With an array, this means adding a new value to an additional slot within the array.
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 63f77cf8-ef91-46a9-a94c-6ed19ec7e7e2
- With an array, this means removing one of the values from the array
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 63f77d09-fe7f-4b1e-a41a-3ce67a90cc59
- Measuring Speed
  ls-type:: annotation
  hl-page:: 25
  hl-color:: yellow
  id:: 63f77d11-414a-4087-8900-208a61486993
- instead in how many steps it takes.
  ls-type:: annotation
  hl-page:: 26
  hl-color:: yellow
  id:: 63f77d23-2ddc-44da-ba89-6f7c184df472
- when we measure how “fast” an operation takes,
  ls-type:: annotation
  hl-page:: 26
  hl-color:: yellow
  id:: 63f77d29-2b63-4499-832b-b5c89230fe80
- Measuring the speed of an operation in terms of time is undependabl
  ls-type:: annotation
  hl-page:: 26
  hl-color:: red
  id:: 63f77d4b-c88f-4342-848e-777408c794bc
  hl-stamp:: 1677163862267
- the time will always change depending on the hardware it is run on.
  ls-type:: annotation
  hl-page:: 26
  hl-color:: red
  id:: 63f77d4d-0bcd-40ff-9712-85ee0f21ae31
  hl-stamp:: 1677163866511
- Why do we measure code’s speed in terms of steps?
  ls-type:: annotation
  hl-page:: 26
  hl-color:: red
  id:: 63f77d51-9e32-4e17-baec-c73223814ee0
  hl-stamp:: 1677163860056
- speed, time complexity, efficiency, performance, and runtime interchangeably. They all refer to the number of steps a given operation takes.
  ls-type:: annotation
  hl-page:: 26
  hl-color:: green
  id:: 63f77d6e-9285-48c6-8b39-0da2dfea4762
  hl-stamp:: 1677163891072
- Reading
  ls-type:: annotation
  hl-page:: 26
  hl-color:: blue
  id:: 63f77d78-9907-4a61-ade7-6ee36c974a43
  hl-stamp:: 1677163899064
- the computer would jump right to index 2 and report that it contains the value "cucumbers".
  ls-type:: annotation
  hl-page:: 26
  hl-color:: blue
  id:: 63f77d8c-b4c4-4edd-bd3a-189edae13464
- When a program declares an array, it allocates a contiguous set of empty cells for use in the program. 
  ls-type:: annotation
  hl-page:: 27
  hl-color:: blue
  id:: 63f77dc3-cddc-43ab-a9d8-9676e7abcdda
- Now, every cell in a computer’s memory has a specific address.
  ls-type:: annotation
  hl-page:: 28
  hl-color:: blue
  id:: 63f77dce-a75b-40d5-9ba8-e3b37b601038
- it can jump straight to that index because of the combination of the following facts about computers:
  ls-type:: annotation
  hl-page:: 28
  hl-color:: blue
  id:: 63f77de7-d86d-4c14-b111-71315255a20f
- ls-type:: annotation
  hl-page:: 28
  hl-color:: blue
  id:: 63f77dfd-b173-4855-a101-641e79dc34a9
  1. A computer can jump to any memory address in one step.
- ls-type:: annotation
  hl-page:: 29
  hl-color:: blue
  id:: 63f77e05-40d1-47c2-be75-62c5bef64b9a
  2. Whenever a computer allocates an array, it also makes note at which memory address the array begins.
- the computer would simply take the memory address at index 0 and add 3.
  ls-type:: annotation
  hl-page:: 29
  hl-color:: blue
  id:: 63f77e20-6915-4135-9087-1d7c753341d5
- Reading from an array is, therefore, an efficient operation
  ls-type:: annotation
  hl-page:: 29
  hl-color:: blue
  id:: 63f77e4e-107f-41e9-a5f9-8592d5ab0a86
- e computer can read any index by jumping to any memory address in one step
  ls-type:: annotation
  hl-page:: 29
  hl-color:: blue
  id:: 63f77e53-63b9-498f-a1c1-4f858dcb829f
- Searching
  ls-type:: annotation
  hl-page:: 29
  hl-color:: purple
  id:: 63f77e77-c937-4a5d-be0f-4049701093a1
  hl-stamp:: 1677164159039
- searching an array means looking to see whether a particular value exists within an array and if so
  ls-type:: annotation
  hl-page:: 29
  hl-color:: purple
  id:: 63f77e90-4eb6-4c65-a30f-35ae93a29d03
- ndex it’s located.
  ls-type:: annotation
  hl-page:: 29
  hl-color:: purple
  id:: 63f77e94-ccc2-40a7-b452-cee1adc5300f
- Searching, though, is tedious, since the computer has no way to jump to a particular value.
  ls-type:: annotation
  hl-page:: 30
  hl-color:: purple
  id:: 63f77eb4-89d0-4429-be10-adc82d6425d2
- it has no idea offhand what values are contained at each memory address.
  ls-type:: annotation
  hl-page:: 30
  hl-color:: purple
  id:: 63f77ee1-0d1d-4f51-9712-7d00edc01a4e
- t for N cells in an array, linear search would take a maximum of N steps
  ls-type:: annotation
  hl-page:: 32
  hl-color:: purple
  id:: 63f77f3d-9501-40f1-bad6-3aa8a69d7675
- Such an insertion takes just one step.
  ls-type:: annotation
  hl-page:: 32
  hl-color:: yellow
  id:: 63f77f5d-a673-4a00-81de-ff1c9b6b2ff5
  hl-stamp:: 1677164384736
- when allocating an array, the computer always keeps track of the array’s size
  ls-type:: annotation
  hl-page:: 32
  hl-color:: yellow
  id:: 63f77f68-6363-4e4b-8b8f-27fbe2160181
- nserting a new piece of data at the beginning or in the middle of an array is a different story
  ls-type:: annotation
  hl-page:: 33
  hl-color:: red
  id:: 63f77fa5-8733-4c35-9d95-cdef3ce72bb9
  hl-stamp:: 1677164472175
- In these cases, we need to shift pieces of data to make room for what we’re inserting, leading to additional steps.
  ls-type:: annotation
  hl-page:: 33
  hl-color:: red
  id:: 63f77fb4-34a7-4ee5-8abf-57f067328b2a
  hl-stamp:: 1677164470592
- The worst-case scenari
  ls-type:: annotation
  hl-page:: 34
  hl-color:: red
  id:: 63f77fef-d119-4d40-a024-f0b670b5b2e4
- the scenario in which insertion takes the most steps
  ls-type:: annotation
  hl-page:: 34
  hl-color:: red
  id:: 63f77ff7-9380-4741-9909-109dfe7ae11f
- insert data at the beginning of the array. 
  ls-type:: annotation
  hl-page:: 34
  hl-color:: red
  id:: 63f7800b-5f99-4280-87c2-9463f77c8755
- we have to move all the other values one cell to the right.
  ls-type:: annotation
  hl-page:: 34
  hl-color:: red
  id:: 63f78011-26f3-43c5-b1b6-1871bac290e3
- Like insertion, the worst-case scenario of deleting an element is deleting the very first element of the array. This is because index 0 would become empty, and we’d have to shift all the remaining elements to the left to fill the gap.
  ls-type:: annotation
  hl-page:: 35
  hl-color:: red
  id:: 63f7900d-c05a-4151-a314-8df8b10d535d
- Why Data Structures Matter
  ls-type:: annotation
  hl-page:: 22
  hl-color:: yellow
  id:: 63f7911c-f361-4cbf-9245-09815d2ba7ab
  hl-stamp:: 1677168931405
- A computer can read from an array in just one step. 
  ls-type:: annotation
  hl-page:: 26
  hl-color:: yellow
  id:: 63f7933f-90a8-4f16-b0f1-1a3cfd21184f
- Sets: How a Single Rule Can Affect Efficiency
  ls-type:: annotation
  hl-page:: 36
  hl-color:: yellow
  id:: 63f79ab0-7249-45bf-a0dc-8884f7ec54a6
- A set is a data structure that does not allow duplicate values to be contained within it.
  ls-type:: annotation
  hl-page:: 36
  hl-color:: yellow
  id:: 63f79ab8-c6f0-4efd-8dbe-c880cd3e9938
- Sets are useful when you need to ensure that you don’t have duplicate data.
  ls-type:: annotation
  hl-page:: 36
  hl-color:: yellow
  id:: 63f79ad2-0fa1-4613-b164-2c0ac85bf7b3
- Reading from a set is exactly the same as reading from an array
  ls-type:: annotation
  hl-page:: 37
  hl-color:: yellow
  id:: 63f79b5f-ce9e-463f-ae9e-01a6968ad1e6
- Searching a set also turns out to be no different than searching an array
  ls-type:: annotation
  hl-page:: 37
  hl-color:: yellow
  id:: 63f79b68-6288-4591-bcce-f02fea8528c1
- Insertion, 
  ls-type:: annotation
  hl-page:: 37
  hl-color:: yellow
  id:: 63f79b6c-ba45-4668-b10c-6f3b1f4b1ef3
- With a set, however, the computer first needs to determine that this value doesn’t already exist in this set—because that’s what sets do: they prevent duplicate data from being inserted into them.
  ls-type:: annotation
  hl-page:: 37
  hl-color:: yellow
  id:: 63f79b88-83ae-4651-87cf-30232b4e3211
- inserting a value at the end of a set,
  ls-type:: annotation
  hl-page:: 37
  hl-color:: yellow
  id:: 63f79b92-1254-443b-b932-ebd04e79d6a7
- every insertion into a set first requires a search.
  ls-type:: annotation
  hl-page:: 37
  hl-color:: yellow
  id:: 63f79bba-39ef-4c23-84d6-c2f6bd69db33
- Inserting a value at the end of a set is the best-case scenario, but we still had to perform six steps for a set originally containing five elements.
  ls-type:: annotation
  hl-page:: 39
  hl-color:: yellow
  id:: 63f79c04-28c5-441d-9ea0-85f8d4f6fcd1
- set will take up to N + 1
  ls-type:: annotation
  hl-page:: 39
  hl-color:: yellow
  id:: 63f79c1a-8d73-4c86-8511-8a69d9075942
- Contrast this with the regular array, in which such an insertion takes a grand total of one step.
  ls-type:: annotation
  hl-page:: 39
  hl-color:: purple
  id:: 63f79c53-2704-4e9d-9fc3-7e69253abe70
  hl-stamp:: 1677171797988
- In the worst-case scenario, where we’re inserting a value at the beginning of a set
  ls-type:: annotation
  hl-page:: 39
  hl-color:: red
  id:: 63f79c5d-5f29-45d6-b73e-90cb03c072e4
  hl-stamp:: 1677171815076
- needs to search N cells
  ls-type:: annotation
  hl-page:: 39
  hl-color:: red
  id:: 63f79c61-576e-4288-b103-7b9c5c1fe69b
  hl-stamp:: 1677171817516
- another N steps to shift all the data to the right, and another final step to insert the new value. 
  ls-type:: annotation
  hl-page:: 39
  hl-color:: red
  id:: 63f79c75-8c60-4c4d-9894-a0e23c363cda
- total of 2N + 1 steps
  ls-type:: annotation
  hl-page:: 39
  hl-color:: red
  id:: 63f79c7a-568e-4373-8bd8-6bd07949735b
- Contrast this to insertion into the beginning of a regular array, which only takes N + 1 steps.
  ls-type:: annotation
  hl-page:: 39
  hl-color:: green
  id:: 63f79c8c-c7e9-43ac-9f1a-add3f6b7bf91
  hl-stamp:: 1677171854860
- You must analyze the needs of your own application and decide which data structure is a better fit.
  ls-type:: annotation
  hl-page:: 39
  hl-color:: green
  id:: 63f79ce0-a4d8-4e58-88d8-fd053f583baf
- Exercises
  ls-type:: annotation
  hl-page:: 40
  hl-color:: green
  id:: 63f7a74f-d0c3-4d0c-a571-84c127a2748a