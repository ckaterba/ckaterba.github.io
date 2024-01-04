###
# naive wordle algorithm
# computer generates word, then tries to guess it implementing wordle rules
# 
###

library(tidyverse)
library(lexicon)

words <- subset(grady_augmented, str_length(grady_augmented) == 5)
words <- subset(words, !str_detect(words,"[:punct:]"))

playWordle <- function(){
  #wordle <- sample(words, 1)
  wordle <- "vivid"
  wL <- str_split(wordle,"")[[1]]
  count <- 1
  guess <- sample(words, 1)
  gL <- str_split(guess,"")[[1]]
  outcome <- 0
  print(str_c("wordle is: ", wordle))
  newWords <- words
  while(count <= 5 ){
    if( guess == wordle){
      outcome <- str_c(guess, " is correct!")
      print(outcome)
      break
    }
    if( guess != wordle){
      count <- count + 1
      outcome <- str_c(guess, " is incorrect.")
      print(outcome)
      exact <- wL == gL #exact character matches
      notIn <- gL[!(gL %in% wL)]
      cont <- as.logical((wL != gL)*(gL %in% wL) ) #in but not exact match
      if(sum(exact)>0){  #if more than one exact match
        patE <- "^"
        for(i in 1:5){
          if(exact[i]){patE <- str_c(patE, gL[i])}
          if(!exact[i]){patE <- str_c(patE, ".")}
        }
        newWords <- subset(newWords, str_detect(newWords, patE)) #restricts to words only with matches where we have em
      }
      for(let in gL[cont]){
        newWords <- subset(newWords, str_detect(newWords, let)) #restricts to words containing letters that match, but aren't exact
      }
      for(let in notIn){
        newWords <- subset(newWords, !str_detect(newWords, let)) #eliminates words containing letters we guessed incorrectly
      }
      guess <- sample(newWords, 1)[[1]]
      gL <- str_split(guess,"")[[1]]
    }
  }
  return(count)
}

# wins <- 0
# games <- 0
# for(i in 1:1000){
#   out <- playWordle()
#   wins <- wins + out
#   games <- games + 1
# }
# 
# print(wins/games)

 # counts <- numeric()
 # for(i in 1:5000){
 #   counts <- append(counts, playWordle())
 # }