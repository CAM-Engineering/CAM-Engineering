(defun c:sayhello ()
  ;; Step 1: Initialize variables (unnecessary complexity)
  (setq first-part "HELLO,")
  (setq second-part "MY")
  (setq third-part "NAME")
  (setq fourth-part "IS")
  (setq fifth-part "CAM")

  ;; Step 2: Introduce pointless intermediate steps
  (setq part1 (strcat first-part " "))
  (setq part2 (strcat part1 second-part " "))
  (setq part3 (strcat part2 third-part " "))
  (setq part4 (strcat part3 fourth-part " "))
  (setq final-message (strcat part4 fifth-part))

  ;; Step 3: Add some more useless steps
  (setq temp1 (strlen final-message))  ;; Find length of the final string
  (setq temp2 (+ temp1 1))             ;; Pointless addition
  (setq temp3 (substr final-message 1 temp1))  ;; Extract whole string

  ;; Step 4: Display the message to the command line
  (princ "\n=====================")
  (princ "\nGreetings Message:")
  (princ "\n=====================")
  (princ "\n")
  (princ temp3)  ;; Print the actual message
  (princ "\n=====================")

  ;; Step 5: Return control to AutoCAD (required)
  (princ)
)
;go away
