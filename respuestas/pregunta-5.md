MATCH (p:Persona)-[:TRABAJA_EN]->(e:Empresa {nombre:"TechCorp"}),
      (p)-[:USA_TECNOLOGIA]->(t:Tecnologia)
RETURN p.nombre AS Persona, t.nombre AS Tecnologia;