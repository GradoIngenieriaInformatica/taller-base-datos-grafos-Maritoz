MATCH (p1:Persona)-[:TRABAJA_CON]->(p2:Persona),
      (p1)-[:VIVE_EN]->(c:Ciudad),
      (p2)-[:VIVE_EN]->(c)
RETURN DISTINCT p1.nombre AS Persona, p2.nombre AS Companero, c.nombre AS Ciudad;