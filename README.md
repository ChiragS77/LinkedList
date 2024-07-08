# LinkedList
This module is about mastering linkedlist
![1593954161024](https://github.com/ChiragS77/LinkedList/assets/142990449/93d8495a-a61f-4a53-821b-88f959fafe8b)

## Linked List

public class LinkedList{

   static class Node{
     int data;
     Node next;

     public Node(int data){
     this.data = data;
     this.next = null;
    }

    public static Node head;
    public static Node tail;

   }

   public static void main(String[] args){
   LinkedList  ll  = new LL();
   ll.head = new Node(2);
   ll.head.next = new Node(3);
   }
}

### Add Node at first

public void addFirst(data){
Node newNode = new Node(data);
if(head == null){
head  = tail =newNode;
return ;
}
newNode.next = head;
head = newNode;
}

### Add Node at Last
public void addLast(data){
Node newNode = new Node(data);
if(tail==null){
head = tail = newNode;
return;
}
tail.next = newNode;
tail = newNode;
}

### Print List
public void print(){
if(head==null){
return ;
}
Node currNode = head;

while(currNode !=null){
system.out.print(" "+currNode.data);
currNode = currNode.next;
}
}

