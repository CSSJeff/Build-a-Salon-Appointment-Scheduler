-- Connect to postgres as freecodecamp user
CREATE DATABASE salon;

\c salon

-- Create customers table
CREATE TABLE customers(
  customer_id SERIAL PRIMARY KEY,
  name VARCHAR(50),
  phone VARCHAR(20) UNIQUE
);

-- Create services table
CREATE TABLE services(
  service_id SERIAL PRIMARY KEY,
  name VARCHAR(50)
);

-- Insert at least 3 services
INSERT INTO services(name) VALUES ('cut');
INSERT INTO services(name) VALUES ('color');
INSERT INTO services(name) VALUES ('style');

-- Create appointments table
CREATE TABLE appointments(
  appointment_id SERIAL PRIMARY KEY,
  customer_id INT REFERENCES customers(customer_id),
  service_id INT REFERENCES services(service_id),
  time VARCHAR(20)
);