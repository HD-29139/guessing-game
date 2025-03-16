### The program randomly generates a secret number between **1 and 100**, and your mission is to guess it! After each guess, you'll receive a hint whether your number is **too small**, **too big**, or **just right**!

#### How to Run

Make sure you have ![Rust](https://img.shields.io/badge/-Rust-000000?style=flat&logo=rust&logoColor=white) installed on your system. If not, get it from [rust-lang.org](https://www.rust-lang.org/).

#### Step 1: Clone the Repository
```bash
git clone https://github.com/HD-29139/guessing-game
cd guessing-game
```
if you're not a simian and have managed to do everything right
#### Step 2: Just run using
```bash
cargo run
```

The game follows these simple steps:

1. **Generate a Secret Number:** Uses the `rand` crate to generate a random number between 1 and 100.
2. **Take User Input:** Prompts the user to enter a guess.
3. **Compare and Respond:** Uses pattern matching to provide feedback:
- Too small
- Too big
- **You win**

#### Dependencies

The game uses the `rand` crate to generate random numbers.
Make sure to add this to your `Cargo.toml`:
```toml
[dependencies]
rand = "0.8.5"
```
or just do:
```bash
cargo add rand
```
more about: [crates.io/rand](https://crates.io/crates/rand).


#### Exemple Output

```yaml
guess the number!
please input your guess:
50
You guessed: 50
too small

please input your guess:
75
You guessed: 75
too big

please input your guess:
63
You guessed: 63
you win
```

### that's all, bye
