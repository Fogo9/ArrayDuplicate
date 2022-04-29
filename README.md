# **ARRAY DUPLICATE**

## INFORMATION

* **Program to find how many times the elements in the array are repeated, that is, their frequencies.**

## TECHNOLOGIES USED

* **JAVA**

## CONTENTS

* List, count, i and j variables are declared with int.

* Arrays class is defined from util library.

* Indicates how many times numbers are repeated using for and if loops.

## CODES

```Java

        import java.util.Arrays;

        public class ArrayDuplicate {


            public static void main(String[] args) {


                int[] list = {10, 20, 20, 10, 10, 20, 5, 20};

                Arrays.sort(list);

                int count = 0;


```

```Java

                for(int i = 0; i < list.length; i++){

                    count = 0;

                    for(int j = 0; j < list.length; j++){

                        if(list[i] == list[j]){

                            count++;

                        }
                    }

                    if(i!=0 && list[i-1]!=list[i]){

                        System.out.println(String.format("The number %d is repeated %d times.", list[i], count));

                    }

                    if(i == 0 && list[i + 1] != list[i]){

                        System.out.println(String.format("The number %d is repeated %d times.", list[i], count));

                    }

                    if(i == 0 && list[i + 1] == list[i]){

                        System.out.println(String.format("The number %d is repeated %d times.", list[i], count));

                    }
                }


            }
        }

```

```bash

    The number 5 is repeated 1 times.
    The number 10 is repeated 3 times.
    The number 20 is repeated 4 times.

```

<br />

## LINK

* Click here https://github.com/Fogo9/ArrayDuplicate.git to access the Github page for this project.

<br />

## LICENSE

* This software is licensed By Tuncay Demir under the MIT license.

<br />

>[Patika.dev](https://app.patika.dev/fogomurphy)

<br/>

| Name |  Email |
| ---- |  ----- |
| Tuncay | tuncaydemir682@gmail.com |
