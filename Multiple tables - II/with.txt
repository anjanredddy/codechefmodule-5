WITH topper AS(  
    SELECT st_name,dept_id
    FROM student
    WHERE  marks> 80
    )
    SELECT topper.st_name,department.dept_name
    FROM topper
    JOIN department
    ON topper.dept_id=department.dept_id;