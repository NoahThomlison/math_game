Requirements
1. Two players
--- Players have 3 lives
--- Players have names, i.e., P1 & P2
2. Each player takes turns answering math questions
3. The math question is genertated each turn by picking two numbers between 1 - 20
4. Players must answer correctly 
5. IF wrong answer, Player will losee a life
6. After each turn the game will output/display the score
7. Game over once a Player has lost all lives
--- Game over = statement of winner and scores


MAIN.rb
- This file will execute all files, i.e. index.

GAME.rb
[] Initalize @turn = 0
[] The turn number will determine who's turn it is
-- P1 = Even # of turns
-- P2 = Odd # of turns
all_players = [player_one, player_two]
--- This Arr will be used to select player to play

class GAME
  ? @game_over = What is this instance Variable ?

  @turn = 0

  def initialize
    @turn += 1
  end

  def self.turn_count
    @turn
  end
end

--- TURN LOGIC ---
(loop) !@game_over do | |
current_player = @players[@turn %2]
other_player = @players[(@turn + 1) % 2

Note: When Game-over is TRUE, game will end



PLAYERS.rb
[] Create 2 Player Classes
[] Each Class will have a default name + starting lives
[] Question: where does the life subtraction logic go? i.e., 'life_counter method'

class PLAYER_ONE
  def initialize
  @player_one = 'Player One'
  @lives = 3
  end

class PLAYER_TWO
  def initialize
  @player_two = 'Player Two'
  @lives = 3
  end
end

QUESTIONS.rb
[] Question: will questions be a class entity?
[] Question: using $stdin.gets.chomp /// gets.chomp for player input
[] Question: ruby method rand(1..20)
[] Question: HOW to do Question Validation to cross check answer provided



