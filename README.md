# student-grades
pseudocode.py
START

DEFINE FUNCTION calculate_average(grades)
    SET total = 0
    FOR each grade IN grades
        total = total + grade
    END FOR
    SET average = total / length of grades
    RETURN average
END FUNCTION

SET students = ["Alice", "Bob", "Carlos"]
SET grades = [
    [90, 85, 88],     # Alice's grades
    [78, 82, 80],     # Bob's grades
    [92, 94, 89]      # Carlos's grades
]

FOR i FROM 0 TO length of students - 1
    PRINT "Grades for", students[i]
    FOR j FROM 0 TO length of grades[i] - 1
        PRINT "  Subject", j + 1, "grade:", grades[i][j]
    END FOR
    avg = calculate_average(grades[i])
    PRINT students[i], "average grade:", avg
END FOR

END
