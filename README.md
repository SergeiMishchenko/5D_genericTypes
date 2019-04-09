# generic types

exercises in using classes that are parameterized with
generic types

## in [`Pair` example](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/2019-04-05_PairOfGenerics)

For each item in this section, find exemplifying code in the `Pair` example.
>For easy reference in the future, take advantage of
GitHub's "Copy permalink" command: click on a line number,
then click on the resulting ellipsis. Use the permalink as the URL
in [GitHub-Flavored Markdown](https://help.github.com/en/articles/basic-writing-and-formatting-syntax#links).


- (an example of this task) the declaration of a `main` method:
```
public static void main(String[] args)
```
in [UserSavedByCompiler](https://github.com/stuyvesant-cs/solutionsHolmes/blob/21b641c9dda3c43d3e71de138c24c29f11687d88/2019-04-05_PairOfGenerics/UserSavedByCompiler.java#L11)


- definition that a class / type that is parameterized by a generic type, `T`:
```
public class Pair<T>
```
in [Pair](https://github.com/stuyvesant-cs/skeletonsHolmes/blob/34c2e635cbaebf480a7906aa63c046c4d9253ca7/5D_genericTypes/FibPair/Pair.java#L8)


- declaration of a variable that can hold a reference to an instance
of such a class:
```
private T first;
```
in [Pair](https://github.com/stuyvesant-cs/skeletonsHolmes/blob/34c2e635cbaebf480a7906aa63c046c4d9253ca7/5D_genericTypes/FibPair/Pair.java#L10)


- assignment to such a variable:
```
this.first =  first;
```
in [Pair](https://github.com/stuyvesant-cs/skeletonsHolmes/blob/34c2e635cbaebf480a7906aa63c046c4d9253ca7/5D_genericTypes/FibPair/Pair.java#L14)


- declaration of a method that returns an instance of such a type:
```
public T getFirst() { return first; }
```
in [Pair](https://github.com/stuyvesant-cs/skeletonsHolmes/blob/34c2e635cbaebf480a7906aa63c046c4d9253ca7/5D_genericTypes/FibPair/Pair.java#L18)


- successful instantiation of an instance of such a class:
```
Pair p2 = new Pair (5, 5); //successful instantiation
```
in [FibPair](https://github.com/SergeiMishchenko/5D_genericTypes/blob/37d17610a28e86137dde5cba4989de4048ac4966/FibPair/FibPair.java#L12)


- *un*successful instantiation of an instance of such a class,
caught by the compiler:
```
// Pair p1 = new Pair <Integer,  ("String"); //unsuccessful instantiation
```
in [FibPair](https://github.com/SergeiMishchenko/5D_genericTypes/blob/37d17610a28e86137dde5cba4989de4048ac4966/FibPair/FibPair.java#L11)


- a variable that can hold a reference to an instance of the generic type
in a class / type that is parameterized by a generic type:
```
		Pair nextPair = new Pair (bigger, smaller);
```
in [FibPair](https://github.com/SergeiMishchenko/5D_genericTypes/blob/00b605e2a0dadc9b27bb0ee24149e41a8d01bfab/FibPair/FibPair.java#L61)


- the declaration of a method or constructor that accepts a parameter of a generic type:
```
    private static Pair nextPairAfter(Pair pair) {
        int bigger = 0; //for errors
		int smaller = 0;
		if (pair.getFirst() instanceof Integer & pair.getSecond() instanceof Integer){
			bigger = (int)pair.getFirst() + (int)pair.getSecond();
			smaller = (int)pair.getFirst();
		}
		return new Pair(bigger, smaller);
    }
```
in [FibPair](https://github.com/SergeiMishchenko/5D_genericTypes/blob/00b605e2a0dadc9b27bb0ee24149e41a8d01bfab/FibPair/FibPair.java#L54)


- the declaration of a method that returns a value of a generic type:
```
    private static Pair nextPairAfter(Pair pair) {
        int bigger = 0; //for errors
		int smaller = 0;
		if (pair.getFirst() instanceof Integer & pair.getSecond() instanceof Integer){
			bigger = (int)pair.getFirst() + (int)pair.getSecond();
			smaller = (int)pair.getFirst();
		}
		return new Pair(bigger, smaller);
    }
```
in [FibPair](https://github.com/SergeiMishchenko/5D_genericTypes/blob/00b605e2a0dadc9b27bb0ee24149e41a8d01bfab/FibPair/FibPair.java#L54)


