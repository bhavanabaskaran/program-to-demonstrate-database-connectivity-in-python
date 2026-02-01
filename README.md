# program-to-demonstrate-database-connectivity-in-python
import mysql.connector
conn=
mysql.connector.connect(host=&#39;localhost&#39;,user=&#39;root&#39;,passwd=&#39;&#39;,database=&#39;db1&#39;)
cursor = conn.cursor()
cursor.execute(&quot;insert into books values (101,&#39;Python&#39;)&quot;)
print(&quot;record inserted successfully&quot;)
cursor.execute(&quot;select * from books&quot;)
result=cursor.fetchall()

print(result)
