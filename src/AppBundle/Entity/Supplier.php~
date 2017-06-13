<?php

namespace AppBundle\Entity;

use Doctrine\ORM\Mapping as ORM;
use Symfony\Component\Validator\Constraints as Assert;

/**
 * Supplier
 * @ORM\Table(name="supplier")
 * @ORM\Entity(repositoryClass="AppBundle\Repository\SupplierRepository")
 */
class Supplier
{
    /**
     * @var int
     *
     * @ORM\Column(name="id", type="integer")
     * @ORM\Id
     * @ORM\GeneratedValue(strategy="AUTO")
     */
    private $id;

    /**
     * @var string
     *
     * @ORM\Column(name="nom", type="string", length=255)
     */
    private $nom;

    /**
     * @var string
     * @Assert\NotEqualTo("")
     * @ORM\Column(name="adress", type="string", length=255)
     */
    private $adress;

    /**
     * @var string
     * @Assert\Email(
     *     message = "Votre email '{{ value }}' n'est pas valide.",
     *     checkMX = true
     * )
     * @ORM\Column(name="email", type="string", length=255)
     */
    private $email;

    /**
     * @var string
     * @Assert\Regex("/[0-9]{5}/")
     *
     * @ORM\Column(name="cp", type="string", length=255)
     */
    private $cp;

    /**
     * @var integer
     * @Assert\Regex("/[A-Za-z -']+/")
     * @ORM\Column(name="ville", type="integer", length=255)
     */
    private $ville;

    /**
     * @var int
     * @Assert\Regex("/[0-9]{3}[ \.\-]?[0-9]{3}[ \.\-]?[0-9]{3}[ \.\-]?[0-9]{5}/")
     * @ORM\Column(name="siret", type="integer")
     */
    private $siret;

    /**
     * @var string
     * @Assert\Regex("/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/")
     * @ORM\Column(name="web_site", type="string", length=255)
     */
    private $webSite;

    /**
     * @var integer
     * @Assert\Regex("/^[0-3]?[0-9]/")
     * @ORM\Column(name="delivery_time", type="integer", length=255)
     */
    private $deliveryTime;

    /**
     * @var int
     * @Assert\Regex("/^[1-5]/")
     * @ORM\Column(name="note", type="integer")
     */
    private $note;


    /**
     * Get id
     *
     * @return int
     */
    public function getId()
    {
        return $this->id;
    }

    /**
     * Set nom
     *
     * @param string $nom
     *
     * @return supplier
     */
    public function setNom($nom)
    {
        $this->nom = $nom;

        return $this;
    }

    /**
     * Get nom
     *
     * @return string
     */
    public function getNom()
    {
        return $this->nom;
    }

    /**
     * Set adress
     *
     * @param string $adress
     *
     * @return supplier
     */
    public function setAdress($adress)
    {
        $this->adress = $adress;

        return $this;
    }

    /**
     * Get adress
     *
     * @return string
     */
    public function getAdress()
    {
        return $this->adress;
    }

    /**
     * Set email
     *
     * @param string $email
     *
     * @return supplier
     */
    public function setEmail($email)
    {
        $this->email = $email;

        return $this;
    }

    /**
     * Get email
     *
     * @return string
     */
    public function getEmail()
    {
        return $this->email;
    }

    /**
     * Set cp
     *
     * @param integer $cp
     *
     * @return supplier
     */
    public function setCp($cp)
    {
        $this->cp = $cp;

        return $this;
    }

    /**
     * Get cp
     *
     * @return integer
     */
    public function getCp()
    {
        return $this->cp;
    }

    /**
     * Set ville
     *
     * @param string $ville
     *
     * @return supplier
     */
    public function setVille($ville)
    {
        $this->ville = $ville;

        return $this;
    }

    /**
     * Get ville
     *
     * @return string
     */
    public function getVille()
    {
        return $this->ville;
    }

    /**
     * Set siret
     *
     * @param integer $siret
     *
     * @return supplier
     */
    public function setSiret($siret)
    {
        $this->siret = $siret;

        return $this;
    }

    /**
     * Get siret
     *
     * @return int
     */
    public function getSiret()
    {
        return $this->siret;
    }

    /**
     * Set webSite
     *
     * @param string $webSite
     *
     * @return supplier
     */
    public function setWebSite($webSite)
    {
        $this->webSite = $webSite;

        return $this;
    }

    /**
     * Get webSite
     *
     * @return string
     */
    public function getWebSite()
    {
        return $this->webSite;
    }

    /**
     * Set deliveryTime
     *
     * @param integer $deliveryTime
     *
     * @return supplier
     */
    public function setDeliveryTime($deliveryTime)
    {
        $this->deliveryTime = $deliveryTime;

        return $this;
    }

    /**
     * Get deliveryTime
     *
     * @return integer
     */
    public function getDeliveryTime()
    {
        return $this->deliveryTime;
    }

    /**
     * Set note
     *
     * @param integer $note
     *
     * @return supplier
     */
    public function setNote($note)
    {
        $this->note = $note;

        return $this;
    }

    /**
     * Get note
     *
     * @return int
     */
    public function getNote()
    {
        return $this->note;
    }
}
