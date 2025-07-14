Attaching the postman collection as .json for readMe

{
	"info": {
		"_postman_id": "4077b8e6-a786-4e09-82fc-7905364a70b7",
		"name": "Products",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json",
		"_exporter_id": "38056204"
	},
	"item": [
		{
			"name": "RegisterUsers",
			"request": {
				"method": "POST",
				"header": [
					{
						"key": "Content-Type",
						"value": "application/json"
					}
				],
				"body": {
					"mode": "raw",
					"raw": "{\n    \"email\": \"john.doe@example.com\",\n    \"password\": \"password123\"\n  }",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:3000/api/auth/register",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "3000",
					"path": [
						"api",
						"auth",
						"register"
					]
				}
			},
			"response": []
		},
		{
			"name": "loginUser",
			"request": {
				"method": "POST",
				"header": [
					{
						"key": "Content-Type",
						"value": "application/json"
					}
				],
				"body": {
					"mode": "raw",
					"raw": "{\n    \"email\": \"john.doe@example.com\",\n    \"password\": \"password123\"\n  }",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:3000/api/auth/login",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "3000",
					"path": [
						"api",
						"auth",
						"login"
					]
				}
			},
			"response": []
		},
		{
			"name": "Get and GetAllProducts",
			"request": {
				"method": "GET",
				"header": [],
				"url": {
					"raw": "http://localhost:3000/api/products/687556bc3258a1419bb031e9",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "3000",
					"path": [
						"api",
						"products",
						"687556bc3258a1419bb031e9"
					]
				}
			},
			"response": []
		},
		{
			"name": "CreateProducts",
			"request": {
				"method": "POST",
				"header": [
					{
						"key": "Content-Type",
						"value": "application/json"
					},
					{
						"key": "Authorization",
						"value": "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2ODc1NTgyYmFmMjEzMjRhYzJhZTIyNjEiLCJpYXQiOjE3NTI1MjA4ODIsImV4cCI6MTc1MzEyNTY4Mn0.ZHsUo_WaCwyTIT8E7HEcHfwotkKkDCWn7_BWHCQZ60Y"
					}
				],
				"body": {
					"mode": "raw",
					"raw": "{\n    \"name\": \"Samsung Galaxy S24\",\n    \"description\": \"Latest Android smartphone with AI features\",\n    \"price\": 849.99,\n    \"category\": \"electronics\"\n  }",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:3000/api/products",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "3000",
					"path": [
						"api",
						"products"
					]
				}
			},
			"response": []
		},
		{
			"name": "updateProducts",
			"request": {
				"method": "PUT",
				"header": [
					{
						"key": "Content-Type",
						"value": "application/json"
					},
					{
						"key": "Authorization",
						"value": "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2ODc1NTgyYmFmMjEzMjRhYzJhZTIyNjEiLCJpYXQiOjE3NTI1MjA4ODIsImV4cCI6MTc1MzEyNTY4Mn0.ZHsUo_WaCwyTIT8E7HEcHfwotkKkDCWn7_BWHCQZ60Y"
					}
				],
				"body": {
					"mode": "raw",
					"raw": "{\n    \"name\": \"Samsung Galaxy S24 Ultra\",\n    \"price\": 1199.99,\n    \"description\": \"Premium Android smartphone with S Pen and advanced camera\"\n  }",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:3000/api/products/687556bc3258a1419bb031e9",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "3000",
					"path": [
						"api",
						"products",
						"687556bc3258a1419bb031e9"
					]
				}
			},
			"response": []
		},
		{
			"name": "deleteProducts",
			"request": {
				"method": "DELETE",
				"header": [
					{
						"key": "Authorization",
						"value": "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2ODc1NTgyYmFmMjEzMjRhYzJhZTIyNjEiLCJpYXQiOjE3NTI1MjA4ODIsImV4cCI6MTc1MzEyNTY4Mn0.ZHsUo_WaCwyTIT8E7HEcHfwotkKkDCWn7_BWHCQZ60Y"
					}
				],
				"url": {
					"raw": "http://localhost:3000/api/products/65f1234567890abcdef12347",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "3000",
					"path": [
						"api",
						"products",
						"65f1234567890abcdef12347"
					]
				}
			},
			"response": []
		}
	]
}
