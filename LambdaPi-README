
Put LambdaPi.hs and prelude.lp in a directory of your choice.

$ ghc --make -o lp LambdaPi.hs
[1 of 1] Compiling LP               ( LP.hs, LP.o )
Linking lp ...
$ ./lp
Interpreter for lambda-Pi.
Type :? for help.
LP> :?
List of commands:  Any command may be abbreviated to :c where
c is the first character in the full name.

<expr>                  evaluate expression
let <var> = <expr>      define variable
assume <var> :: <expr>  assume variable

:type <expr>            print type of expression
:browse                 browse names in scope
:load <file>            load program from file
:quit                   exit interpreter
:help, :?               display this list of commands
LP> :l prelude.lp

[... lots of type signatures ...]

LP> plus 40 2
42 :: Nat
LP> :t fromto
forall x :: Nat . Vec Nat x
LP> fromto 3
Cons Nat 2 2 (Cons Nat 1 1 (Cons Nat 0 0 (Nil Nat))) :: Vec Nat 3
LP> let v = fromto 3
v :: Vec Nat 3
LP> :t at
forall (x :: *) (y :: Nat) (z :: Vec x y) (a :: Fin y) . x
LP> at Nat 3 v (FSucc 2 (FZero 1))
1 :: Nat
LP> :q

