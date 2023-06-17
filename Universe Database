--
-- PostgreSQL database dump
--

-- Dumped from database version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)
-- Dumped by pg_dump version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

DROP DATABASE universe;
--
-- Name: universe; Type: DATABASE; Schema: -; Owner: freecodecamp
--

CREATE DATABASE universe WITH TEMPLATE = template0 ENCODING = 'UTF8' LC_COLLATE = 'C.UTF-8' LC_CTYPE = 'C.UTF-8';


ALTER DATABASE universe OWNER TO freecodecamp;

\connect universe

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: galaxy; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.galaxy (
    galaxy_id integer NOT NULL,
    speed integer,
    description text,
    name character varying(255) NOT NULL,
    galaxy_shape character varying(255)
);


ALTER TABLE public.galaxy OWNER TO freecodecamp;

--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.galaxy_galaxy_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.galaxy_galaxy_id_seq OWNER TO freecodecamp;

--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.galaxy_galaxy_id_seq OWNED BY public.galaxy.galaxy_id;


--
-- Name: moon; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.moon (
    moon_id integer NOT NULL,
    name character varying(255) NOT NULL,
    has_water boolean NOT NULL,
    planet_id integer NOT NULL,
    name_code character varying(255) NOT NULL
);


ALTER TABLE public.moon OWNER TO freecodecamp;

--
-- Name: moon_moon_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.moon_moon_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.moon_moon_id_seq OWNER TO freecodecamp;

--
-- Name: moon_moon_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.moon_moon_id_seq OWNED BY public.moon.moon_id;


--
-- Name: nebulosas; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.nebulosas (
    nebulosas_id integer NOT NULL,
    name character varying(255) NOT NULL,
    type character varying(255) NOT NULL,
    distance numeric NOT NULL,
    description text NOT NULL
);


ALTER TABLE public.nebulosas OWNER TO freecodecamp;

--
-- Name: nebulosas_nebulosas_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.nebulosas_nebulosas_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.nebulosas_nebulosas_id_seq OWNER TO freecodecamp;

--
-- Name: nebulosas_nebulosas_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.nebulosas_nebulosas_id_seq OWNED BY public.nebulosas.nebulosas_id;


--
-- Name: planet; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.planet (
    planet_id integer NOT NULL,
    name character varying(255) NOT NULL,
    amount_of_people numeric,
    time_travel boolean DEFAULT false NOT NULL,
    star_id integer NOT NULL
);


ALTER TABLE public.planet OWNER TO freecodecamp;

--
-- Name: planet_planet_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.planet_planet_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.planet_planet_id_seq OWNER TO freecodecamp;

--
-- Name: planet_planet_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.planet_planet_id_seq OWNED BY public.planet.planet_id;


--
-- Name: star; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.star (
    star_id integer NOT NULL,
    radius integer NOT NULL,
    color character varying(255) NOT NULL,
    name character varying(255) NOT NULL,
    galaxy_id integer
);


ALTER TABLE public.star OWNER TO freecodecamp;

--
-- Name: star_star_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.star_star_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.star_star_id_seq OWNER TO freecodecamp;

--
-- Name: star_star_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.star_star_id_seq OWNED BY public.star.star_id;


--
-- Name: galaxy galaxy_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy ALTER COLUMN galaxy_id SET DEFAULT nextval('public.galaxy_galaxy_id_seq'::regclass);


--
-- Name: moon moon_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon ALTER COLUMN moon_id SET DEFAULT nextval('public.moon_moon_id_seq'::regclass);


--
-- Name: nebulosas nebulosas_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.nebulosas ALTER COLUMN nebulosas_id SET DEFAULT nextval('public.nebulosas_nebulosas_id_seq'::regclass);


--
-- Name: planet planet_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet ALTER COLUMN planet_id SET DEFAULT nextval('public.planet_planet_id_seq'::regclass);


--
-- Name: star star_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star ALTER COLUMN star_id SET DEFAULT nextval('public.star_star_id_seq'::regclass);


--
-- Data for Name: galaxy; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.galaxy VALUES (1, NULL, NULL, 'andromeda', NULL);
INSERT INTO public.galaxy VALUES (2, NULL, NULL, 'Via lactea', NULL);
INSERT INTO public.galaxy VALUES (3, NULL, NULL, 'Enana Eliptica de Sagitario', NULL);
INSERT INTO public.galaxy VALUES (4, NULL, NULL, 'Gran nube de Magallanes', NULL);
INSERT INTO public.galaxy VALUES (5, NULL, NULL, 'Galaxia del Sombrero', NULL);
INSERT INTO public.galaxy VALUES (6, NULL, NULL, 'Galaxia del Remolino', NULL);


--
-- Data for Name: moon; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.moon VALUES (1, 'Luna', true, 1, 'moon1');
INSERT INTO public.moon VALUES (2, 'Europa', true, 5, 'moon2');
INSERT INTO public.moon VALUES (5, 'Titan', true, 8, 'moon3');
INSERT INTO public.moon VALUES (6, 'Titan', true, 4, 'moon4');
INSERT INTO public.moon VALUES (7, 'Encelado', true, 8, 'moon5');
INSERT INTO public.moon VALUES (8, 'IO', true, 2, 'moon6');
INSERT INTO public.moon VALUES (10, 'moon', true, 1, 'moon7');
INSERT INTO public.moon VALUES (11, 'cuspide', true, 1, 'moon8');
INSERT INTO public.moon VALUES (12, 'Fobos', true, 3, 'moon9');
INSERT INTO public.moon VALUES (13, 'Miranda', false, 6, 'moon10');
INSERT INTO public.moon VALUES (15, 'Mimas', false, 8, 'moon11');
INSERT INTO public.moon VALUES (16, 'Calisto', false, 5, 'moon12');
INSERT INTO public.moon VALUES (17, 'Deimos', false, 3, 'moon13');
INSERT INTO public.moon VALUES (18, 'Dione', false, 8, 'moon14');
INSERT INTO public.moon VALUES (19, 'Japeto', false, 8, 'moon15');
INSERT INTO public.moon VALUES (20, 'Caronte', false, 9, 'moon16');
INSERT INTO public.moon VALUES (21, 'Rea', false, 8, 'moon17');
INSERT INTO public.moon VALUES (22, 'Nereida', false, 4, 'moon18');
INSERT INTO public.moon VALUES (23, 'Oberon', false, 6, 'moon19');
INSERT INTO public.moon VALUES (24, 'Ganimedes', false, 5, 'moon20');


--
-- Data for Name: nebulosas; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.nebulosas VALUES (1, 'Nebulosa A', 'Emision', 10000, 'Nebulosa de emisión de colores vivos');
INSERT INTO public.nebulosas VALUES (2, 'Nebulosa B', 'Reflexion', 2000, 'Nebulosa que refleja la luz de la estrella mas cercana');
INSERT INTO public.nebulosas VALUES (3, 'Nebulosa C', 'Planetaria', 5000, 'Nebulosa expulsada por una estrella moribunda');


--
-- Data for Name: planet; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.planet VALUES (1, 'Tierra', NULL, false, 1);
INSERT INTO public.planet VALUES (2, 'Mercurio', NULL, false, 1);
INSERT INTO public.planet VALUES (3, 'Marte', NULL, false, 2);
INSERT INTO public.planet VALUES (4, 'Neptuno', NULL, false, 2);
INSERT INTO public.planet VALUES (5, 'Jupiter', NULL, false, 2);
INSERT INTO public.planet VALUES (6, 'Urano', NULL, false, 3);
INSERT INTO public.planet VALUES (7, 'Venus', NULL, false, 3);
INSERT INTO public.planet VALUES (8, 'Saturno', NULL, false, 1);
INSERT INTO public.planet VALUES (9, 'Pluton', NULL, false, 1);
INSERT INTO public.planet VALUES (10, 'Eris', NULL, false, 1);
INSERT INTO public.planet VALUES (11, 'Makemake', NULL, false, 1);
INSERT INTO public.planet VALUES (12, 'Haumea', NULL, false, 1);
INSERT INTO public.planet VALUES (13, 'Ceres', NULL, false, 1);
INSERT INTO public.planet VALUES (14, 'Sedna', NULL, false, 1);
INSERT INTO public.planet VALUES (15, 'Orcus', NULL, false, 1);


--
-- Data for Name: star; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.star VALUES (1, 1234561234, 'red', 'beatlejuice', 1);
INSERT INTO public.star VALUES (2, 1538494, 'yellow', 'joel', 1);
INSERT INTO public.star VALUES (3, 1694, 'yellow', 'big yellow', 1);
INSERT INTO public.star VALUES (4, 169489399, 'orange', 'small orange', 1);
INSERT INTO public.star VALUES (5, 169489399, 'orange', 'star in galaxy 2', 2);
INSERT INTO public.star VALUES (6, 169489399, 'green', 'gary', 2);


--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.galaxy_galaxy_id_seq', 9, true);


--
-- Name: moon_moon_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.moon_moon_id_seq', 24, true);


--
-- Name: nebulosas_nebulosas_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.nebulosas_nebulosas_id_seq', 3, true);


--
-- Name: planet_planet_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.planet_planet_id_seq', 15, true);


--
-- Name: star_star_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.star_star_id_seq', 6, true);


--
-- Name: galaxy galaxy_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_pkey PRIMARY KEY (galaxy_id);


--
-- Name: moon moon_name_code_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_name_code_key UNIQUE (name_code);


--
-- Name: moon moon_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_pkey PRIMARY KEY (moon_id);


--
-- Name: planet name; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT name UNIQUE (name);


--
-- Name: galaxy name_unique; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT name_unique UNIQUE (name);


--
-- Name: nebulosas name_unique_nebulosa; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.nebulosas
    ADD CONSTRAINT name_unique_nebulosa UNIQUE (name);


--
-- Name: star name_unique_star; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT name_unique_star UNIQUE (name);


--
-- Name: nebulosas nebulosas_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.nebulosas
    ADD CONSTRAINT nebulosas_pkey PRIMARY KEY (nebulosas_id);


--
-- Name: planet planet_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_pkey PRIMARY KEY (planet_id);


--
-- Name: star star_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_pkey PRIMARY KEY (star_id);


--
-- Name: star fk_galaxy; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT fk_galaxy FOREIGN KEY (galaxy_id) REFERENCES public.galaxy(galaxy_id);


--
-- Name: moon fk_planet; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT fk_planet FOREIGN KEY (planet_id) REFERENCES public.planet(planet_id);


--
-- Name: planet fk_star; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT fk_star FOREIGN KEY (star_id) REFERENCES public.star(star_id);


--
-- PostgreSQL database dump complete
--
