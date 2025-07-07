# -z_case_example.abap
REPORT z_case_example.

DATA: lv_grade TYPE c VALUE 'B'.

CASE lv_grade.
  WHEN 'A'.
    WRITE: / 'Excellent!'.
  WHEN 'B'.
    WRITE: / 'Very Good!'.
  WHEN 'C'.
    WRITE: / 'Good'.
  WHEN OTHERS.
    WRITE: / 'Try harder next time!'.
ENDCASE.
