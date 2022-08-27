# Music_Player_using_LL
Academic Project under Data Structures and Algorithms course

![image](https://user-images.githubusercontent.com/67479922/187017338-8fa27591-37db-4c0c-8c7e-33dbdd59502f.png)


As part of my CO252 project, I created a Music Player system using the Data Structures and Algorithms: mainly Doubly Linked List, stacks, and queues on C++. This music player can also be used to read and create song items from files. I have also optimized the program by using "itemCount" variable by updating it each and every time a song is added or deleted from the playlist, which removes the need for counting items in linked list (which we all know takes O(n) time), so it improves the time complexity of that function from O(n) to O(1). While it may be more annoying in the short term to update the item count value depending on the operation, there is a performance bonus from doing this. The major part of the challenge included making a doubly linked list that would accept string data and store it efficiently. Involving the usage of file handling was another challenge, to retrieve songs from a pre-made list and adding it to the linked list (current playlist). It also enabled me to write the new input songs to the file. All changes in the list were reflected on the "playlist.txt" file (automatically created while running the program).

Programming Language used: C++
Data Structures used: Linked Lists, Stacks, and Queues

![image](https://user-images.githubusercontent.com/67479922/187017381-2f3fd79f-7c2d-4764-8517-eae4fb8c4148.png)

PROJECT METHODOLOGY / FLOW OF EVENTS:

![MusicPlayerLL_Flowchart](https://user-images.githubusercontent.com/67479922/187017509-ab0a108c-fb56-4cc1-81e9-b118198e9856.jpg)

DIFFERENT FUNCTIONS USED:

1. tofile() –
Function to work on playslist.txt.
2. add_node() –
Function that adds songs to the list using a linked list.
3. add_node_file() –
Function that adds songs to the playlist to linked list from the data passed in addplaylist()
function.
4. delete_file() –
Function to delete song from text file playlist.txt.
5. del_node() –
Function that deletes the last song from the input linked list.
6. printlist() –
Function that displays the input songs of the playlist.
7. count_nodes() –
Function that tracks the number of inputs in the linked list.
8. del_pos() –
Function that deletes songs from the linked list using the position of that song.
9. search1() –
Function that takes song input and linearly searches through the linked list and finds matching
case.
10. push() –
Function that pushes the last played track of play() function into a stack to store and create a
recently played list.
11. display() -
Function to display the stack generated in push() function.
12. play() -
Function to search input song and show if it can be played. It then passes the song to push()
function to be added to recently played list.
13. recent() -
Function that calls display() function.
14. topelement() –
Function that displays the last played song.
15. addplaylist() –
Function that opens text file playlist.txt and passes data to add_node_file() function.
16. del_search() –
Function to search input song and delete it from the list.
17. deletemenu() –
Function to invoke del_search() or del_pos() functions depending on user input.
18. main() –
Function that invokes all other functions of the project based on user defined input.
